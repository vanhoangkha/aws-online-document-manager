# Online Document Manager - Amplify Demo

A web storage solution built with AWS Amplify that enables authenticated users to store, access, and share various types of files (documents, photos, videos) from anywhere with an internet connection. The application features file organization capabilities, backup functionality, and both private and public file sharing options through an intuitive user interface.

## Key Features

- File storage and organization
- Public and private file sharing
- User authentication
- Cloud backup

## Technology Stack

- **AWS Amplify**: Core development toolset providing backend cloud services integration
- **Cloudscape Design System**: Open-source design system for creating web applications, originally developed for AWS services
- **AWS Services**:
  - Amazon S3 (Storage)
  - Amazon Cognito (Authentication)
  - Amazon Comprehend (Text Analysis)
  - Amazon Textract (Document Processing)

## Prerequisites

Before you begin, ensure you have the following installed:

- AWS Account with Access Key and Secret Access Key
- Node.js and npm
- JavaScript IDE
- AWS CLI
- Amplify CLI

## Installation and Setup

1. Install Node.js and npm:
   - Download and install from [Node.js website](https://nodejs.org/en/download/)
   - Verify installation: 
     ```bash
     node -v  # Should be version 12.x or greater
     npm -v   # Should be version 6.x or greater
     ```

2. Set up AWS credentials:
   - Create an [IAM user](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html) in your AWS account
   - Configure user permissions following the [principle of least privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege)
   - Generate and securely store Access Key and Secret Access Key

3. Install required tools:
   ```bash
   # Install AWS CLI
   # Follow instructions at: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

   # Install Amplify CLI
   # Follow instructions at: https://docs.amplify.aws/cli/start/install/
   ```

4. Project setup:
   ```bash
   # Clone the repository
   git clone https://github.com/aws-samples/online-document-manager-amplify

   # Alternative: download source code directly

   # Install dependencies
   cd online-document-manager-amplify
   npm install
   ```

5. Initialize and deploy:
   ```bash
   # Initialize Amplify
   amplify init

   # Deploy backend resources
   amplify push

   # Deploy UI to Amplify Hosting
   amplify publish
   ```

## AWS Amplify Features Used

### Amplify Storage
Provides app content storage capabilities backed by Amazon S3

### Amplify Authentication
Configures authentication and authorization workflows using Amazon Cognito

### Amplify Predictions
Enables AI/ML capabilities for features such as:
- Text recognition from images
- Entity recognition
- Object labeling
- Text interpretation and transcription

### Amplify Hosting
Enables continuous deployment and hosting with git-based workflow

## Security Note

Always keep your AWS Access Key and Secret Access Key secure and never share them publicly or with unauthorized individuals.

## Additional Resources

- [AWS Amplify Documentation](https://docs.amplify.aws/)
- [Cloudscape Design System](https://cloudscape.design/)