## API Report File for "@firebase/performance"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { FirebaseApp } from '@firebase/app';

// @public
export interface FirebasePerformance {
    app: FirebaseApp;
    dataCollectionEnabled: boolean;
    instrumentationEnabled: boolean;
}

// @public
export function getPerformance(app?: FirebaseApp): FirebasePerformance;

// @public
export function initializePerformance(app: FirebaseApp, settings?: PerformanceSettings): FirebasePerformance;

// @public
export interface PerformanceSettings {
    dataCollectionEnabled?: boolean;
    instrumentationEnabled?: boolean;
}

// @public
export interface PerformanceTrace {
    getAttribute(attr: string): string | undefined;
    getAttributes(): {
        [key: string]: string;
    };
    getMetric(metricName: string): number;
    incrementMetric(metricName: string, num?: number): void;
    putAttribute(attr: string, value: string): void;
    putMetric(metricName: string, num: number): void;
    record(startTime: number, duration: number, options?: {
        metrics?: {
            [key: string]: number;
        };
        attributes?: {
            [key: string]: string;
        };
    }): void;
    removeAttribute(attr: string): void;
    start(): void;
    stop(): void;
}

// @public
export function trace(performance: FirebasePerformance, name: string): PerformanceTrace;


```