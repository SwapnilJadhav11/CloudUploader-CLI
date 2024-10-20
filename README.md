# CloudUploader-CLI

## Overview

CloudUploader-CLI is a robust, bash-based Command Line Interface (CLI) tool designed to streamline the process of uploading files to cloud storage solutions. This tool provides a seamless upload experience, similar to popular storage services, with a focus on simplicity and efficiency.

## Features

- Quick and easy file uploads to specified cloud storage (AWS S3)
- Secure handling of authentication and credentials
- Progress tracking for uploads
- Generates shareable links for uploaded files
- File synchronization capabilities
- Support for various file types, including PDFs

## Prerequisites

- Bash shell (version 4.0 or later)
- AWS CLI installed and configured
- An active AWS account with S3 access

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/SwapnilJadhav11/CloudUploader-CLI.git
   cd CloudUploader-CLI
   ```

2. Make the script executable:
   ```
   chmod +x clouduploader
   ```

3. (Optional) Move the script to a directory in your PATH for system-wide access:
   ```
   sudo mv clouduploader /usr/local/bin/
   ```

## Configuration

1. Ensure your AWS CLI is configured with the necessary credentials:
   ```
   aws configure
   ```

2. Set up your S3 bucket (if not already created):
   ```
   aws s3 mb s3://your-bucket-name
   ```

3. Update the `BUCKET_NAME` variable in the `clouduploader` script with your S3 bucket name.

## Usage

Basic usage:
```
clouduploader /path/to/file.txt
```

Options:
- `-h` or `--help`: Display help information
- `-v` or `--version`: Display version information

## Examples

1. Upload a file:
   ```
   clouduploader /path/to/document.pdf
   ```

2. Upload and generate a shareable link:
   ```
   clouduploader /path/to/image.jpg --share
   ```

## Troubleshooting

- Ensure your AWS credentials are correctly configured
- Check that your IAM user has the necessary S3 permissions
- Verify that the specified S3 bucket exists and is accessible


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- AWS for providing the S3 service and SDK
- The open-source community for inspiration and support

## Contact

For support or queries, please open an issue in the GitHub repository.

---

Developed as part of the Cloud Computing Capstone Project.