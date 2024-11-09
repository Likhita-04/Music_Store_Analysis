

---

# Music Database Schema

## Project Overview

This project involves the design of a relational database schema for managing a music library. The database stores information about artists, albums, tracks, playlists, invoices, and customers, providing a structure suitable for a music streaming service or media store. 

## Database Schema

The schema is organized into several key entities, each representing a different aspect of the music library:

1. **Artist**: Stores information about artists.
2. **Album**: Contains albums created by artists.
3. **Track**: Represents individual tracks, including metadata such as genre and media type.
4. **Playlist**: Enables users to create playlists by linking multiple tracks.
5. **Invoice**: Contains billing details related to customer purchases.
6. **Customer**: Holds customer information.
7. **Employee**: Manages employee information, possibly for customer support or sales.

## Entity-Relationship (ER) Diagram

Below are the ER diagrams representing the schema:

### Detailed Schema Diagram
![Music Database Schema](MusicDatabaseSchema.png)

### Simplified Schema Diagram
![Simplified Schema Diagram](schema_diagram.png)

### Key Relationships

- **Artist to Album**: An artist can create multiple albums.
- **Album to Track**: Each album consists of multiple tracks.
- **Track to MediaType & Genre**: Tracks have associated media types and genres.
- **Invoice to Customer**: Each invoice is linked to a customer.
- **InvoiceLine**: Contains details about each item in an invoice.
- **PlaylistTrack**: A junction table allowing tracks to be added to multiple playlists.

## Files in This Repository

- **MusicDatabaseSchema.png**: ER diagram showcasing all entities and relationships in the database.
- **schema_diagram.png**: Alternative ER diagram for visualizing the structure.

## Usage

This schema is useful for building applications that manage large music libraries, such as streaming services or online music stores. The schema supports:

- User-specific playlists
- Detailed metadata for tracks
- Billing and invoice management
- Customer relationship management

## Getting Started

To use this schema, you can import it into a database management system like MySQL, PostgreSQL, or SQLite. Each table includes primary keys, foreign keys, and indices for efficient querying.

