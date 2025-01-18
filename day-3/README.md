# E-commerce Marketplace - Day 3 API Integration

## Overview
This repository contains Day 3 implementation of the E-commerce Marketplace Hackathon 2025, focusing on API integration and data migration into Sanity CMS. The project demonstrates data migration from external API to Sanity CMS and integration with Next.js frontend.

## Project Structure
```
├── data-migration-project/
│   ├── node_modules/
│   ├── data.js             # Migration script
│   └── package.json
│
├── e-commerce-project/     # Main Next.js + Sanity Project
│   ├── app/
│   │   ├── page.tsx
│   │   └── products/[slug]/page.tsx
│   ├── sanity/
│   │   └── schemas/
│   │       └── product.ts
│   ├── components/
│   │   └── ProductList.tsx
│   └── lib/
│       └── sanity.query.ts
```

## Implementation Steps

### 1. Data Migration
- Cloned the API source project
- Created migration script (data.js)
- Used Node.js to migrate data to Sanity CMS
- Verified data migration in Sanity Studio

### 2. Main Project Setup
- Created new Next.js project
- Installed and configured Sanity
- Created product schema based on migrated data
- Set up Vision GROQ queries for data fetching

### 3. Frontend Integration
- Implemented product listing page
- Created dynamic product detail pages
- Used GROQ queries to fetch data from Sanity
- Tested API endpoints using Thunder Client

## Tech Stack
- Next.js 14
- Sanity CMS
- TypeScript
- Node.js (for data migration)
- Thunder Client (API testing)

## Setup Instructions

### Data Migration Setup
```bash
# Clone the API source project
git clone [api-source-repo]

# Install dependencies
npm install

# Run migration script
node data.js
```

### Main Project Setup
```bash
# Create new Next.js project
npx create-next-app@latest

# Install Sanity
npm install -D @sanity/vision @sanity/cli

# Start development server
npm run dev
```

## Environment Variables
```
NEXT_PUBLIC_SANITY_PROJECT_ID=your_project_id
NEXT_PUBLIC_SANITY_DATASET=your_dataset
SANITY_API_TOKEN=your_api_token
```

## API Integration
- Used GROQ queries for data fetching
- Implemented in sanity.query.ts
- Tested endpoints using Thunder Client
- Rendered data in product pages

## Best Practices Implemented
- Secure environment variable usage
- Clean code structure
- Error handling
- Data validation
- Version control with meaningful commits

## Future Improvements
- Add search functionality
- Implement filtering system
- Add pagination
- Enhance loading states
- Add more product details

## Contributing
1. Fork the repository
2. Create your feature branch (git checkout -b feature/YourFeature)
3. Commit your changes (git commit -m 'Add some feature')
4. Push to the branch (git push origin feature/YourFeature)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgments
- Hackathon organizers and mentors
- API providers
- Sanity CMS documentation
- Template providers