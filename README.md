
# LabLens - Health AI System

A production-ready Health AI application with comprehensive BMAD (Biomarker Monitoring and Analysis Dashboard) capabilities.

## Features

- **Advanced Health Analytics**: Real-time biomarker monitoring and analysis
- **AI-Powered Insights**: Intelligent health recommendations using OpenAI and AbacusAI
- **Secure Data Management**: Supabase integration with robust security practices
- **Comprehensive Testing**: Full test suite for reliability and quality assurance
- **Production-Ready**: Optimized for deployment with proper security configurations

## Tech Stack

- **Frontend**: Next.js 14, React, TypeScript, Tailwind CSS
- **Backend**: Supabase (PostgreSQL, Auth, Storage)
- **AI Services**: OpenAI GPT-4, AbacusAI
- **Testing**: Jest, React Testing Library
- **Deployment**: Vercel-ready with production optimizations

## Quick Start

### Prerequisites

- Node.js 18+ 
- npm or yarn
- Supabase account
- OpenAI API key
- AbacusAI account

### Installation

1. Clone the repository:
```bash
git clone https://github.com/biospark33/lablens.git
cd lablens
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env.local
```

4. Configure your environment variables in `.env.local`:
```
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
SUPABASE_SERVICE_ROLE_KEY=
OPENAI_API_KEY=
ABACUS_API_KEY=
ABACUS_API_ENDPOINT=
```

5. Run the development server:
```bash
npm run dev
```

## Environment Variables

Create a `.env.local` file with the following variables:

| Variable | Description | Required |
|----------|-------------|----------|
| `NEXT_PUBLIC_SUPABASE_URL` | Your Supabase project URL | Yes |
| `NEXT_PUBLIC_SUPABASE_ANON_KEY` | Supabase anonymous key | Yes |
| `SUPABASE_SERVICE_ROLE_KEY` | Supabase service role key | Yes |
| `OPENAI_API_KEY` | OpenAI API key for AI features | Yes |
| `ABACUS_API_KEY` | AbacusAI API key | Yes |
| `ABACUS_API_ENDPOINT` | AbacusAI endpoint URL | Yes |

## Production Deployment

### Vercel Deployment

1. Connect your GitHub repository to Vercel
2. Configure environment variables in Vercel dashboard
3. Deploy with automatic builds on push

### Manual Deployment

1. Build the application:
```bash
npm run build
```

2. Start the production server:
```bash
npm start
```

## Testing

Run the test suite:

```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage

# Run integration tests
npm run test:integration
```

## Project Structure

```
├── app/                    # Next.js app directory
├── components/            # Reusable UI components
├── lib/                   # Utility libraries and configurations
│   ├── supabase.ts       # Supabase client configuration
│   ├── openai.ts         # OpenAI integration
│   └── abacus.ts         # AbacusAI integration
├── scripts/              # Testing and utility scripts
├── docs/                 # Documentation
├── public/               # Static assets
└── types/                # TypeScript type definitions
```

## Security

- Environment variables are properly configured and excluded from version control
- Supabase Row Level Security (RLS) policies implemented
- API routes secured with proper authentication
- Input validation and sanitization throughout the application

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and questions, please open an issue in the GitHub repository.
