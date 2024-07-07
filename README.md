# Pinakas

> "Pinakas" means "board" in Greek.
> A web monitoring tool, dashboard and system to visualize an area (city, region, country etc) status by displaying several **indicators**.

## Structure

### Menu

- Home
- Account
- About
- Contact
- Legal terms
- Data
- API

## Categories (of Data - Cards)

- Weather
- Transportation
- Traffic & roads
- Business
- Hospitals
- Pharmacy
- Events
- News
- Alerts (emergency)
- Police alerts & security
- Sports
- NOW (what is happening now in the area)
- Live streaming
- Entertainment
- Housing (stats)
- Education stats
- Gov services contact and info
- Population
- Electricity
- Financial stats
- Interner services status
- Phone services status
- Water supply
- Banks and financial institutions
- Financial indicators
- Social media
- Queues on public sector services (e.g. in hospitals)
- Trends (in social or news)

## Features & Technical

- HTML emded
- Sharing widgets
- Dashboard generator
- Data snapshots (static exports)
- API (JSONAPI, GraphQL)
- NoSQL database
- Oauth login
- Social account login
- User accounts
- JSON described (fields, relationships, uuid etc)
- Search with filters
- Live edit Cards (inline)
- Print
- RDF, schemaorg triages
- OpenStreetMaps (mapping)
- Icon fonts (svg)
- Live streaming (camera stream)
- Frontend with JS
- Backend (Drupal)

## Structure & entities

- User
- Card (data display widget)
- Feed (import resource)
  - CSV
  - RSS
  - User input
  - JSON API
  - log files
  - HTML parser
- Report (multiple Cards with texts etc)
- API consumer
- Dashboard (of Cards)
- Page (normal HTML)
- Export

## Card widgets

- Text
- Table display
- Numerical data
  - Plain numbers
  - Percent
  - Diffs
  - Diagrams
  - On/Off
  - Live number change
- Location
  - maps
  - pins
  - routes
- iframe

## Card options

- Permissions
- Live edit (click to edit)
- Highlight effect (on new values)
- Dynamic color change by value
- Drag and drop on Dashboard
- Show/Hide
- Change display
- Grow (grid and columns)
- Change details of display (minimal, short, normal, extended, detailed)
- Export to JSON
- Print to image
- Snapshot
- Clone/copy
- Lock (no changes allowed etc)

## Example

### JSON of a Card

  ```JSON
{
  "type": "list_integer",
  "status": 1,
  "frequency": [
    1,
    15,
    30
  ],
  "owner": 123,
  "uuid": "56771d54-10d8-4516-90c2-1efe796550f7",
  "created": 11232433214,
  "changed": 11232433214,
  "area": "Thessaloniki, Greece",
  "taxonomy": [
    "gov",
    "thessaloniki"
  ],
  "data": {
    "εφορία": 23,
    "κεπ": 3,
    "λεωφορεία": 2
  }
}
  ```

### Indicators examples

- Date and time
- Weather (by time, alerts)
- Locations with safety issues
- Business new vs closed
- Transportation status and info (bus, taxi, train, airplanes, bicycles)
- Technical works on roads
- Road incidents
- Calls to the Police/Fire service
- Live events now
- Status of the water (quality of water, limits)
- Population (births, deaths)
