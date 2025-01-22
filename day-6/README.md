# Deployment Preparation and Staging Environment Setup

## Overview
This repository contains all activities, files, and documentation from Day 6 of the deployment preparation process. The primary focus was setting up a staging environment, conducting rigorous testing, and ensuring readiness for deployment.

## Objectives
- Prepare the marketplace for deployment
- Set up a staging environment using **Vercel**
- Configure and secure environment variables
- Validate application functionality in a production-like environment
- Conduct functional, performance, and security testing
- Document and organize project files

## Key Activities

### 1. Staging Environment Setup
- Selected **Vercel** as the hosting platform
- Connected GitHub repository to the hosting platform
- Configured build and deployment settings
- Secured environment variables using `.env` files and hosting platform settings

### 2. Testing
- **Functional Testing**: Verified workflows (e.g., product listings, cart operations)
- **Performance Testing**: Used **Lighthouse** to measure speed and responsiveness
- **Security Testing**: Validated HTTPS, secure APIs, and input fields
- Documented all test cases in a CSV format

### 3. Documentation
- Created a structured folder hierarchy for easy navigation
- Summarized all project activities in a **README.md** file

## Project Structure
```
.
├── documents/
│   ├── Day1_Documentation.pdf
│   ├── Day2_Deployment_Checklist.pdf
│   ├── Day6_Test_Cases.csv
│   └── Performance_Report.pdf
├── src/
│   ├── components/
│   ├── pages/
│   └── utils/
├── public/
│   └── assets/
├── .env
├── README.md
└── package.json
```

## Testing Summary

### Test Case Report

| Test Case ID | Description | Expected Result | Actual Result | Status |
|--------------|-------------|-----------------|---------------|---------|
| TC001 | Validate product listing | Products displayed | Products displayed | Passed |
| TC002 | API error handling | Show fallback message | Fallback message shown | Passed |
| TC003 | Cart functionality | Cart updates correctly | Cart updates correctly | Passed |
| TC004 | Responsive layout | Layout adjusts properly | Layout adjusts properly | Passed |

### Performance Results
- **Lighthouse Score**:
  - Performance: 100
  - Accessibility: 77
  - Best Practices: 93
  - SEO: 91

## Next Steps
- Resolve any documented issues from testing
- Optimize for production deployment
- Transition to the production environment

## Submission

### Required Artifacts:
1. Link to the deployed staging environment
2. GitHub repository with:
   - Documents folder containing all project-related documentation
   - Test case reports in CSV format
   - Performance testing results
   - Organized project files

## Acknowledgments
Special thanks to **Ameen Alam** for the guidance and resources provided during this stage.