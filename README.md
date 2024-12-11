# Expo Camera onBarCodeScanned Intermittency Bug

This repository demonstrates a bug where the `onBarCodeScanned` function of Expo's Camera API fails to consistently trigger barcode scan events. The issue appears to be related to performance or race conditions, resulting in intermittent or completely missing barcode detections.  The bug is difficult to reliably reproduce, making debugging challenging.

## Bug Reproduction Steps

1. Clone this repository.
2. Install dependencies: `npm install` or `yarn install`
3. Run the app: `expo start`
4. Point the camera at barcodes. Observe that sometimes barcodes are detected, other times they are missed, even with the same barcode and lighting conditions.

## Solution

A potential solution involves modifying the barcode detection settings (types, precision, etc.) or incorporating error handling and retry mechanisms.  However, a more robust solution from the Expo team addressing the underlying performance issues is needed to resolve this inconsistently reproducible problem.