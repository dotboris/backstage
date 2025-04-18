## API Report File for "@backstage/release-manifests"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
// @public
export function getManifestByReleaseLine(
  options: GetManifestByReleaseLineOptions,
): Promise<ReleaseManifest>;

// @public
export type GetManifestByReleaseLineOptions = {
  releaseLine: string;
};

// @public
export function getManifestByVersion(
  options: GetManifestByVersionOptions,
): Promise<ReleaseManifest>;

// @public
export type GetManifestByVersionOptions = {
  version: string;
  fetch?: (
    url: string,
    options?: {
      signal?: AbortSignal;
    },
  ) => Promise<Pick<Response, 'status' | 'json' | 'url'>>;
};

// @public
export type ReleaseManifest = {
  releaseVersion: string;
  packages: {
    name: string;
    version: string;
  }[];
};
```
