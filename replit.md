# Cybersecurity Cheatsheet Manager

## Overview

This is a fully functional web application designed to manage cybersecurity cheatsheets and reference materials. The application features a complete hacker-themed interface with role-based access control, premium features, and comprehensive user management. It includes PIN-based authentication, local storage for data persistence, and admin capabilities for managing users and permissions. Users can create, edit, organize, and search through cybersecurity cheatsheets with markdown-style formatting support.

## User Preferences

- Preferred communication style: Simple, everyday language
- Authentication: PIN-based security (PIN: 909913) 
- Theme: Hacker-style color scheme (green/black matrix theme)
- User Identity: BitMonk (displayed in welcome message)
- No external dependencies - everything runs locally from index.html

## System Architecture

### Frontend Architecture
- **Technology**: Pure HTML/CSS/JavaScript (vanilla web technologies)
- **Structure**: Single-page application with responsive design
- **Styling**: Custom CSS with gradient backgrounds and modern UI components
- **Layout**: Flexbox-based layout system for responsive design

### Backend Architecture
- **Current State**: No backend implementation present
- **Anticipated**: Will likely need a backend API for data persistence and management
- **Potential Technologies**: Node.js/Express or similar lightweight server framework

### Data Storage
- **Current State**: No database implementation
- **Anticipated**: Will need persistent storage for cheatsheet data
- **Potential Solution**: May use Drizzle ORM for database operations

## Key Components

### Authentication System
- **Dual Authentication Mode**: Separate login systems for users and admin access
- **User Authentication**: Username and password-based login for standard users
- **Admin Authentication**: PIN-based access (909913) for administrator privileges
- **Role-Based Access Control**: Admin and standard user roles with different privileges
- **User Registration**: Account creation system with username and password validation
- **Session Management**: localStorage-based authentication with user identity persistence
- **Profile Management**: User profile with password change functionality and logout option
- **Access Type Selector**: Tabbed interface to switch between user login and admin access
- **Welcome Popup**: Personalized greeting showing current user's name with animated glow effect

### User Interface Components
- **Header Section**: Hacker-themed gradient header with Matrix-style green/black colors
- **Authentication Screen**: Full-screen PIN entry with error handling
- **Sidebar**: Search functionality, add button, and cheatsheet list with hacker styling
- **Main Content Area**: Text editor with toolbar and formatting options
- **Modal Dialogs**: Add cheatsheet modal with consistent hacker theme
- **Responsive Design**: Mobile-first approach with viewport meta tag

### Implemented Features
- ✓ Dual authentication system (Username/Password for users, PIN for admin)
- ✓ Tabbed login interface with user and admin access modes
- ✓ User account creation with password validation (minimum 6 characters)
- ✓ Password change functionality accessible from user profile
- ✓ User profile section with logout capability
- ✓ Role-based authentication system (Admin/User roles)
- ✓ Premium feature access control (theme customization)
- ✓ Admin panel with comprehensive user management capabilities
- ✓ Permission-based UI visibility (buttons show/hide based on access)
- ✓ Multi-theme system (6 color themes) restricted to premium users
- ✓ Cheatsheet creation with custom naming
- ✓ Rich text editor with markdown-style formatting toolbar
- ✓ Real-time search functionality
- ✓ Auto-save functionality (1-second delay after typing)
- ✓ Local storage data persistence for users and cheatsheets
- ✓ Delete cheatsheet functionality
- ✓ Export cheatsheets as .txt files with metadata
- ✓ Storage usage calculator and information display
- ✓ Enhanced keyboard navigation for all forms and modals
- ✓ Hacker-themed UI with multiple color schemes

## Data Flow

### Current State
- Static HTML page with embedded CSS
- No dynamic data flow implemented yet

### Anticipated Flow
1. User authentication and session management
2. CRUD operations for cheatsheet management
3. Search and filtering capabilities
4. Data persistence to database

## External Dependencies

### Current Dependencies
- None (vanilla HTML/CSS)

### Potential Future Dependencies
- Database system (PostgreSQL likely with Drizzle ORM)
- Authentication service
- Frontend framework (if complexity increases)
- Build tools and bundlers

## Deployment Strategy

### Current State
- Simple static file hosting capable
- Can be deployed to any web server

### Future Considerations
- Will need full-stack hosting when backend is implemented
- Environment configuration for database connections
- Static asset optimization
- SSL/HTTPS implementation for security

## Development Notes

The application is in very early development with only basic HTML structure in place. The CSS styling suggests a modern, professional interface with:
- Responsive design principles
- Modern color schemes (gradient backgrounds)
- Clean typography using system fonts
- Flexible layout system

The incomplete HTML file shows the beginning of a main content area with flexbox layout, indicating plans for a multi-section interface. Future development will likely focus on implementing JavaScript functionality, backend API development, and database integration for persistent cheatsheet storage.