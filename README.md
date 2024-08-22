# Pwopryo

Pwopryo is an integrated platform designed to streamline the process of renting and leasing properties in Haiti.

## The Solution: Pwopryo, your all-in-one property rental and leasing platform

- **Comprehensive Listings**: Manage and explore property listings with detailed information and images.
- **User Management**: Handle user authentication, profiles, and favorites.
- **Communication**: Integrated messaging system for direct user interactions.
- **Advanced Search and Filtering**: Find properties based on specific criteria and preferences.
- **Reviews and Ratings**: Users can leave feedback and rate properties.
- **Favorites Management**: Save and revisit your favorite properties.

## Open Source, Open Architecture

- **Frontend**: Built with React.js and Tailwind CSS for a responsive and modern user interface.
- **Backend**: Powered by AdonisJs and PostgreSQL for robust server-side functionality.
- **Deployment**: Both frontend and backend can be deployed independently with Docker and Traefik support.

## ✨ Features

- **Property Listings**: Display properties with detailed information, images, and availability status.
- **User Profiles**: Manage user accounts, favorites, and communication.
- **Search and Filtering**: Easily find properties using advanced search options.
- **Responsive Design**: Optimized for various devices and screen sizes.
- **Interactive UI**: Includes animations and smooth transitions for a better user experience.

## 💻 Deploy Locally

### Requirements

- Docker
- Docker Compose
- Git

### Run the Application

To get started with Pwopryo, follow these steps:

1. **Clone the Repository**:

   ```bash
   # Clone the repository
   git clone https://github.com/pwopryo/pwopryo.git
   cd pwopryo
   ```

2. **Run with Docker**:

   ```bash
   # Start the frontend and the backend with Docker
   docker-compose -f docker-compose.yml up -d

   # Create and migrate the database
   docker-compose exec [backend_container_name] node ace migration:run
   docker-compose exec [backend_container_name] node ace db:seed
   ```

3. **Access the Application**:

   You can now open your browser and navigate to:
   - **Frontend**: [http://localhost:5173](http://localhost:5173)
   - **Backend API**: [http://localhost:3333](http://localhost:3333)

**Note**: Replace `[backend_container_name]` with the actual container name for the backend. You can find this by running `docker ps` and looking for the container name.
