# @essentx/elementaris-api-schema

This package contains type definitins for public endpoints and their available methods, request bodies and response schemas.
It is intended to be used when developing an application which is working against the elementaris API.

## Installation

```sh
npm install --save-dev @essentx/elementaris-api-schema
```

## Usage

```ts
import type { paths } from "@essentx/elementaris-api-schema";

async function getSbomReportById(
  id: string
): Promise<paths["/sbom/reports/{id}"]["get"]["responses"][200]> {
  // ...
}
```

### With generics

```ts
import type { paths } from "@essentx/elementaris-api-schema";

async function request<
  TUrl extends keyof paths,
  TMethod extends keyof paths[TUrl],
  TBody extends paths[TUrl][TMethod]["parameters"]
>(url: TUrl, method: TMethod, body?: TBody) {
  const res = await fetch(url, {
    method,
    body: body ? JSON.stringify(body) : undefined,
  });

  // do something with the response
}
```
