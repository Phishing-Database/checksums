# Checksums

This repository provides checksum files for the Phishing.Database project. These checksums ensure the integrity of the files published or updated as part of the project.

## Format

Each time a new file is published to [phish.co.za](https://phish.co.za) or an existing file is updated in the Phishing Database project, the corresponding checksum files are updated or published in this repository.

These files follow these naming conventions, where `filename` refers to the file you want to verify:

- `filename.md5`
- `filename.sha1`
- `filename.sha256`
- `filename.sha512`

## Usage

For every file in the Phishing Database project, you can find its associated checksum files in this repository. These checksum files can be used to verify the integrity and authenticity of the downloaded files.

### Linux

Use the following commands to verify a file against its checksum:

- **MD5**:
  ```bash
  md5sum -c filename.md5
  ```
- **SHA1**:
  ```bash
  sha1sum -c filename.sha1
  ```
- **SHA256**:
  ```bash
  sha256sum -c filename.sha256
  ```
- **SHA512**:
  ```bash
  sha512sum -c filename.sha512
  ```

### macOS

On macOS, you can use the following commands in the Terminal. The `shasum` command supports multiple algorithms via the `-a` flag:

- **MD5**:
  ```bash
  md5 filename
  ```
  Compare the output with the contents of `filename.md5`.

- **SHA1**:
  ```bash
  shasum -a 1 filename
  ```
  Compare the output with the contents of `filename.sha1`.

- **SHA256**:
  ```bash
  shasum -a 256 filename
  ```
  Compare the output with the contents of `filename.sha256`.

- **SHA512**:
  ```bash
  shasum -a 512 filename
  ```
  Compare the output with the contents of `filename.sha512`.

### Windows

1. Open Command Prompt (CMD).
2. Navigate to the folder containing the file and checksum.
3. Run the following commands:

- **MD5**:
  ```cmd
  certutil -hashfile filename MD5
  ```
- **SHA1**:
  ```cmd
  certutil -hashfile filename SHA1
  ```
- **SHA256**:
  ```cmd
  certutil -hashfile filename SHA256
  ```
- **SHA512**:
  ```cmd
  certutil -hashfile filename SHA512
  ```

Compare the output of the above commands with the content of the checksum files to ensure integrity.

## Authors

- **Mitchell Krog** ([GitHub: @mitchellkrogza](https://github.com/mitchellkrogza)) - Support **@mitchellkrogza** on [Ko-fi](https://ko-fi.com/mitchellkrogza)!

- **Nissar Chababy** ([GitHub: @funilrys](https://github.com/funilrys)) - Sponsor **@funilrys** via [GitHub Sponsors](https://github.com/sponsors/funilrys)!

- **Phishing Database Contributors**

## License

```
MIT License

Copyright (c) 2018-2024 Mitchell Krog - @mitchellkrogza
Copyright (c) 2018-2024 Nissar Chababy - @funilrys

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```