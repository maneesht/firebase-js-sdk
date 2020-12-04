## API Report File for "@firebase/functions-exp"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { FirebaseApp } from '@firebase/app-types-exp';
import { Functions } from '@firebase/functions-types-exp';
import { HttpsCallable } from '@firebase/functions-types-exp';
import { HttpsCallableOptions } from '@firebase/functions-types-exp';

// @public
export function getFunctions(app: FirebaseApp, regionOrCustomDomain?: string): Functions;

// @public
export function httpsCallable(functionsInstance: Functions, name: string, options?: HttpsCallableOptions): HttpsCallable;

// @public
export function useFunctionsEmulator(functionsInstance: Functions, host: string, port: number): void;


// (No @packageDocumentation comment for this package)

```