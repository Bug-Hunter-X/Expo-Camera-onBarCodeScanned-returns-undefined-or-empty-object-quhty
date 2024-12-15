# Expo Camera onBarCodeScanned returns undefined or empty object

This repository demonstrates a bug in Expo's Camera API where the `onBarCodeScanned` function sometimes returns `undefined` or an empty object instead of the expected barcode data. This inconsistency makes reliable barcode scanning difficult.

## Bug Description
The `onBarCodeScanned` function within Expo's Camera API is designed to provide barcode data when a barcode is scanned. However, in certain instances, it unpredictably returns `undefined` or an empty object, even when a barcode is clearly detected by the camera.

## Reproduction
To reproduce the issue, clone this repository and run the `bug.js` example. You will likely encounter scenarios where barcode scans result in no data being returned.

## Solution
The provided `bugSolution.js` demonstrates a workaround to mitigate this issue by adding more robust error handling and data validation.  The solution carefully checks the received data before processing to handle cases where it's undefined or an empty object. 

## Contributing
Contributions are welcome!  If you have additional insights or a more comprehensive solution, please submit a pull request. 