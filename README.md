# Review Request Management Application

## Overview

The Review Request Management Application is a ServiceNow application designed to enable Enterprise Architects to assign users to tasks above the Demand during the Ideation process. This application streamlines the review and assignment workflow for strategic initiatives and project requests.

## Current Status

🚧 **Development in Progress** 🚧

This application is currently in active development. We are building out the core functionality and features. The current implementation includes basic incident management capabilities that will serve as the foundation for the review request system.

## Features

### Current Features
- **Incident Management Interface**: A React-based user interface for managing incidents
- **Basic CRUD Operations**: Create, read, update, and delete incident records
- **ServiceNow Integration**: Full integration with ServiceNow platform using Now SDK Fluent
- **Responsive Design**: Modern, responsive web interface

### Planned Features
- **Review Request Workflow**: Complete workflow for review request management
- **User Assignment**: Capability for Enterprise Architects to assign users to specific tasks
- **Demand Integration**: Integration with ServiceNow Demand Management
- **Approval Process**: Multi-stage approval workflow
- **Dashboard and Reporting**: Analytics and reporting capabilities

## Architecture

### Technology Stack
- **Frontend**: React 19.x with modern JSX components
- **Backend**: ServiceNow Now Platform with Now SDK Fluent 4.2.0
- **Development Language**: ServiceNow Fluent DSL (TypeScript-based)
- **Application Scope**: `x_220772_rev_req`

### Project Structure
```
src/
├── client/                 # React frontend components
│   ├── app.jsx            # Main application component
│   ├── main.jsx           # Application entry point
│   ├── components/        # Reusable React components
│   │   ├── IncidentForm.jsx
│   │   └── IncidentList.jsx
│   └── services/          # API service layer
│       └── IncidentService.js
└── fluent/                # ServiceNow Fluent metadata
    ├── index.now.ts       # Main Fluent entry point
    └── ui-pages/          # UI Page definitions
        └── incident-manager.now.ts
```

## Development Setup

### Prerequisites
- ServiceNow Now SDK 4.2.0 or higher
- Node.js (version compatible with React 19.x)
- Access to a ServiceNow development instance

### Installation
1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

### Building the Application
```bash
npm run build
```

### Deployment
Deploy to your ServiceNow instance:
```bash
npm run deploy
```

### Development Scripts
- `npm run build` - Build the application
- `npm run deploy` - Deploy to ServiceNow instance
- `npm run transform` - Transform source code
- `npm run types` - Generate type definitions

## Application Access

Once deployed, the application can be accessed through:
- **UI Page**: `x_220772_rev_req_incident_manager.do`
- **Direct URL**: Available through ServiceNow navigation

## Contributing

This application is currently under active development. Core features are being built incrementally to support the review request management workflow.

### Development Guidelines
- All ServiceNow metadata should be defined using Fluent DSL in `.now.ts` files
- React components should follow modern functional component patterns
- Maintain separation between client-side and server-side logic

## Roadmap

### Phase 1 (Current)
- ✅ Basic project structure and build system
- ✅ React frontend foundation
- ✅ ServiceNow integration setup
- 🚧 Core incident management functionality

### Phase 2 (Next)
- 🔄 Review request data model
- 🔄 User assignment workflows
- 🔄 Enterprise Architect role-based access

### Phase 3 (Future)
- ⏳ Demand management integration
- ⏳ Approval workflows
- ⏳ Reporting and analytics

## License

UNLICENSED - Internal enterprise application

## Support

For questions or issues during development, please contact the development team or create an issue in the project repository.

---

*This README will be updated as new features are implemented and the application evolves.*