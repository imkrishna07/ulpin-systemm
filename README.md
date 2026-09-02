# 3D ULPIN — Urban Land & Property Intelligence System

Live Demo
Live Website: https://stellar-seahorse-216141.netlify.app/

A web-based **3D cadastral visualization and vertical property intelligence platform** designed to represent urban land parcels, multi-storey buildings, individual property units, and underground infrastructure in a unified 3D environment.

The project is built as a demonstration frontend for the **3D ULPIN (Urban Land & Property Intelligence System)** concept, with an Amritsar Urban Zone demonstration area.

---

## Overview

Traditional 2D cadastral systems primarily represent land parcels on the surface. Modern cities, however, contain increasingly complex vertical properties such as apartments, commercial buildings, elevated infrastructure, and underground utilities.

**3D ULPIN** provides a visual interface for representing these different spatial layers together.

The current frontend demonstrates:

* 3D land parcels
* Multi-storey buildings
* Individual vertical property units
* Property and building information
* Underground infrastructure
* Elevated metro corridors
* Layer-based visualization
* 2D / 3D viewing modes
* Wireframe visualization
* Property search
* AI-assisted analysis simulation
* Topology validation simulation
* Property registry
* Cadastral analytics dashboard

---

## Key Features

### 3D Cadastre

Interactive 3D visualization of the demonstration area using WebGL.

Users can:

* Rotate the scene
* Zoom in and out
* Select parcels
* Select buildings
* Select individual floors
* Inspect vertical property information

### Layer Management

The interface provides independent visualization controls for:

* Surface Parcels
* Buildings
* Apartments
* Roads
* Parking
* Underground Utilities
* Metro / Elevated Corridors
* Terrain
* Property Boundaries

### Vertical Property Representation

Buildings are represented as multiple floor volumes rather than a single 2D footprint.

Selecting a building provides information such as:

* Building name
* Building ID
* Parcel association
* Height
* Number of floors
* Construction type
* Built-up area
* Floor register

Individual floors can also be selected to display vertical property information.

### Underground Infrastructure

The demonstration includes underground spatial assets such as:

* Water infrastructure
* Utility corridors
* Metro tunnels

An **Underground Cutaway** mode allows these assets to be visualized beneath the surface.

### Property Search

The application provides a search interface for finding:

* ULPIN identifiers
* Parcel IDs
* Buildings

Search results can directly open the corresponding property in the 3D cadastre.

### AI-Assisted Analysis

The current prototype includes an interface demonstrating AI-assisted cadastral analysis.

The demo displays simulated results for:

* Building extraction
* Floor segmentation
* Parcel boundary extraction

Example demonstration accuracy values are displayed within the interface.

### Topology Validation

The prototype includes a topology validation workflow that demonstrates checks such as:

* Overlapping parcels
* Building containment
* Floor alignment
* Vertical boundary validity

### Analytics Dashboard

The dashboard provides demonstration metrics including:

* Land parcels
* 3D mapped buildings
* Vertical properties
* Underground assets
* 3D coverage
* Survey accuracy

### Property Registry

A searchable-style property registry displays sample records containing:

* 3D ULPIN
* Parcel ID
* Building
* Floor
* Unit
* Area
* Property type
* Registration status

---

## Technology Stack

### Frontend

* **TypeScript**
* **React**
* **HTML5**
* **CSS3**

### 3D Visualization

* **Three.js**
* **React Three Fiber**
* **React Three Drei**

### UI Icons

* **Lucide React**

### Development & Build

* **Vite**
* **TypeScript Compiler**
* **npm**

The project is configured as a Vite application and uses React 18 with Three.js-related packages.

---

## Project Structure

```text
3d-ulpin-command-center/
│
├── src/
│   ├── App.tsx
│   ├── data.ts
│   ├── main.tsx
│   └── style.css
│
├── index.html
├── package.json
├── package-lock.json
├── tsconfig.json
├── tsconfig.node.json
├── vite.config.ts
├── .gitignore
└── README.md
```

### Important Files

| File             | Purpose                                  |
| ---------------- | ---------------------------------------- |
| `src/App.tsx`    | Main React application and UI components |
| `src/data.ts`    | Demonstration parcel and building data   |
| `src/main.tsx`   | React application entry point            |
| `src/style.css`  | Application styling                      |
| `index.html`     | HTML entry point                         |
| `package.json`   | Dependencies and npm scripts             |
| `vite.config.ts` | Vite configuration                       |
| `tsconfig.json`  | TypeScript configuration                 |

The application's entry point loads `src/main.tsx`, which initializes the React application and imports the main stylesheet.

---

The frontend contains sample:

* 25 parcels
* 12 buildings
* Multiple floors and vertical units
* Underground assets
* Urban infrastructure

The parcel and building datasets are currently defined directly in `src/data.ts`.

The data is intended to demonstrate the application's visualization and interaction model rather than represent an official cadastral database.

---

## Application Architecture

```text
                 3D ULPIN
                     │
        ┌────────────┼────────────┐
        │            │            │
     Cadastre    Registry     Analytics
        │            │            │
        └────────────┼────────────┘
                     │
              React Frontend
                     │
          React Three Fiber
                     │
                 Three.js
                     │
               WebGL / 3D
```

---

## Demonstration Workflow

```text
Select Urban Zone
        ↓
Explore 3D Cadastre
        ↓
Select Surface Parcel
        ↓
View Associated Building
        ↓
Explore Building Floors
        ↓
Select Vertical Property Unit
        ↓
Inspect Property Information
        ↓
Enable Underground Layers
        ↓
Run Analysis / Validation
```

---

## Future Development

The current repository represents the **frontend prototype**. A production implementation can extend the system with:

* Real cadastral databases
* Government land records integration
* Real ULPIN generation and validation
* GIS data integration
* Real 3D building models
* LiDAR and drone data processing
* Digital elevation models
* Floor-plan ingestion
* Real underground utility datasets
* Spatial databases such as PostGIS
* Backend APIs
* Authentication and authorization
* Real AI-based building and floor extraction
* Real topology validation
* Government data interoperability
* Audit trails and ownership history

---

## Project Status

**Status: Frontend Prototype / Demonstration**

The current implementation focuses on demonstrating the **user interface, 3D cadastral visualization, vertical property representation, registry workflow, and analytics experience**.

Backend services, live government datasets, authentication, and production cadastral validation are not part of the current frontend implementation.

---

## Use Case

The concept is intended to support urban land administration by providing a unified spatial representation of:

```text
Land Parcel
     │
     ├── Building
     │      │
     │      ├── Floor 1
     │      │      ├── Unit A
     │      │      └── Unit B
     │      │
     │      ├── Floor 2
     │      │      ├── Unit A
     │      │      └── Unit B
     │      │
     │      └── ...
     │
     ├── Underground Assets
     │
     └── Infrastructure / Right-of-Way
```

This allows property relationships to be represented across **surface, vertical, and underground dimensions** rather than only through conventional 2D parcels.

---

## Team

Developed as a prototype project for **Smart India Hackathon 2026**.

**Project:** 3D ULPIN — Urban Land & Property Intelligence System

---

## License

This project is currently intended for educational, research, and hackathon demonstration purposes.
