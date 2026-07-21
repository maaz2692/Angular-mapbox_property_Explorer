# Mapbox Project Navigator

**Author:** Maaz Mustafa Khurshed Qazi
**Version:** 1.0.0

Mapbox Project Navigator is a modern, interactive real-estate web application built with **Angular**, **TypeScript**, and **Mapbox GL JS**.

The application allows users to explore property projects, view high-quality images, navigate between project-detail pages, and interact with a dynamic Mapbox-powered map.

The application loads structured project data from JSON sources and presents information such as:

* Project images
* Location coordinates
* City, province, and project metadata
* Detailed project information
* Interactive map locations
* Custom SVG map markers

Angular’s modular architecture supports reusable components, smooth routing, maintainable code, and a responsive user experience.

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 20.3.5.

## Technology Stack

* Angular
* TypeScript
* Mapbox GL JS
* HTML5
* CSS
* Angular Router
* JSON-based data sources

## Project Structure

```text
src/
├── app/
│   ├── components/        # Reusable user-interface components
│   ├── pages/             # Application pages and route-level views
│   ├── services/          # Data loading and application services
│   ├── models/            # TypeScript interfaces and data models
│   └── app.routes.ts      # Application routing configuration
├── assets/
│   ├── data/              # JSON-based property and project data
│   ├── images/            # Property and interface images
│   └── markers/           # Custom SVG map markers
├── environments/
│   └── environment.example.ts
├── styles.css             # Global application styles
└── main.ts                # Application entry point
```

## Application Flow

1. The application loads structured property data from JSON sources.
2. Angular services provide the data to reusable components and project pages.
3. Property locations are displayed on a Mapbox-powered interactive map.
4. Custom SVG markers identify individual projects.
5. Angular Router handles navigation between the map, project listings, and detail pages.
6. Environment configuration supplies the Mapbox access token without exposing it in the repository.


## Clone the Repository

```bash
git clone https://github.com/maaz2692/mapbox.git
cd mapbox
```

## Install Dependencies

```bash
npm install
```

## Configure the Mapbox Access Token

Before running the application, create the following file:

```text
src/environments/environment.ts
```

Add your Mapbox access token:

```typescript
export const environment = {
  production: false,
  mapbox: {
    accessToken: 'YOUR_MAPBOX_ACCESS_TOKEN_HERE'
  }
};
```

For the production build, create:

```text
src/environments/environment.prod.ts
```

Add the production configuration:

```typescript
export const environment = {
  production: true,
  mapbox: {
    accessToken: 'YOUR_MAPBOX_ACCESS_TOKEN_HERE'
  }
};
```

You can create a Mapbox access token through the [Mapbox account dashboard](https://account.mapbox.com/).

> Do not commit a private or production access token to the repository.

## Development Server

Start the local development server:

```bash
ng serve
```

Once the server is running, open:

```text
http://localhost:4200/
```

The application will automatically reload whenever you modify the source files.

## Code Scaffolding

To generate a new Angular component, run:

```bash
ng generate component component-name
```

For a complete list of available Angular schematics, run:

```bash
ng generate --help
```

## Production Build

Build the application by running:

```bash
ng build
```

The compiled application will be stored in the:

```text
dist/
```

directory.

The production build applies Angular optimizations to improve application performance.

## Running Unit Tests

Run the configured unit tests with:

```bash
ng test
```

## Project Highlights

This project demonstrates:

* Development of reusable Angular and TypeScript components
* Integration of interactive maps using Mapbox GL JS
* Loading and presenting structured JSON data
* Creation of custom SVG map markers
* Implementation of project-detail pages
* Client-side routing with Angular Router
* Development of data-heavy and location-based interfaces
* Environment-based configuration for development and production

## Future Improvements

* Add advanced property filtering and search
* Improve mobile responsiveness
* Add loading and error states
* Connect the application to a live REST API
* Add automated end-to-end testing
* Improve accessibility and keyboard navigation
* Deploy a publicly accessible demonstration

## Additional Resources

For more information about Angular CLI commands, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli).

## Author

**Maaz Mustafa Khurshed Qazi**

* [LinkedIn](https://www.linkedin.com/in/qazi-maaz/)
* [GitHub](https://github.com/maaz2692)

## License

This project is available for educational and portfolio purposes.
