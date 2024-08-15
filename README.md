# NativeAOT-Signatures

This repository contains signature files (.sig) for .NET applications compiled with NativeAOT. These signatures are generated using IDA Pro to assist in the reverse engineering of binaries that leverage extensive native methods.

## Usage

1. **Download the Signature File:**
   Navigate to the `signatures` directory, find the signature file corresponding to your version of the binary, and download it.

2. **Applying Signatures in IDA:**
   - Open your binary in IDA.
   - Go to `File` > `Load File` > `FLIRT Signature File...`.
   - Select the downloaded `.sig` file to apply the signatures to your binary.

## Contributing

Contributions to this repository are welcome. Please follow these steps to contribute:
- Fork the repository.
- Create a new branch for your signatures (`git checkout -b your-signature-branch`).
- Add your signature files in the correct directory with appropriate naming conventions.
- Push your changes and open a pull request.

## Signature Files Format and Naming Conventions

- **File Naming:** Each signature file should be named according to the following format: `AppName_Version.sig`
  - For example, `MyApp_1.0.sig`
- **File Versioning:** Each update or new addition should include a version bump in the filename to reflect the binary version it supports.

## Versions and Standards

Each signature file must adhere to the following standards:
- Must be compatible with IDA Pro version 9.0 or higher.
- Should only include signatures that do not infringe on proprietary code or violate software licensing.

## License

This project is released under the MIT License. See the `LICENSE` file for more details.

