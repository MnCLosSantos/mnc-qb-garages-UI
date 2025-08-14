# mnc-qb-garages-UI
qb-garages
A comprehensive garage system for QBCore-based FiveM servers, allowing players to store, retrieve, and manage vehicles with a highly customizable user interface offering 18 unique UI options.
Features

Vehicle Management: Store and retrieve vehicles in public, private, job-specific, and gang-specific garages.
Customizable UI: Choose from 18 distinct UI styles to match your server's aesthetic.
Garage Types: Supports multiple garage types (public, private, job, gang, and impound).
Vehicle State Tracking: Tracks vehicle condition, fuel, and modifications.
Integration: Seamlessly integrates with QBCore framework.
Performance Optimized: Lightweight and optimized for high-performance servers.

Installation

Download the Resource:
Clone or download the qb-garages resource from the repository.


Add to Server:
Place the qb-garages folder in your server's resources directory.


Update Server Config:
Add ensure qb-garages to your server.cfg after qb-core.


Configure Database:
Import the provided sql.sql file into your database to set up necessary tables.


Customize Configuration:
Edit config.lua to set up garage locations, types, and UI preferences.


Restart Server:
Restart your server or use refresh followed by start qb-garages.



Configuration
The main configuration file is config.lua. Key settings include:

Garage Locations: Define coordinates and types for each garage.
Vehicle Limits: Set storage limits for different garage types.
UI Options: Select from 18 UI styles (see below for details).
Job/Gang Restrictions: Restrict access to specific garages based on job or gang.

Example configuration snippet:
Config.UIStyle = "modern-dark" -- Choose from 18 UI styles
Config.Garages = {
    ["main_garage"] = {
        type = "public",
        coords = vector3(123.45, 678.90, 12.34),
        spawnPoint = vector4(123.45, 678.90, 12.34, 90.0),
        maxVehicles = 10
    }
}

UI Customization Options
The qb-garages resource offers 18 UI styles to enhance the player experience. Each style can be set in config.lua using the Config.UIStyle variable. Available options are:

modern-dark: Sleek dark theme with neon accents.
modern-light: Clean light theme with minimalistic design.
retro: Pixelated, 80s-inspired interface.
cyberpunk: Neon-heavy, futuristic aesthetic.
classic: Simple, no-frills design with neutral colors.
luxury: Elegant gold and black theme.
industrial: Gritty, metallic look with bold fonts.
minimal: Ultra-simplified interface with flat design.
vintage: Old-school, sepia-toned design.
holographic: Sci-fi inspired with translucent elements.
neon-glow: Bright neon colors with glowing effects.
monochrome: Single-color scheme with high contrast.
futuristic: High-tech interface with animated elements.
rustic: Wooden textures with a cozy feel.
corporate: Professional, business-like design.
arcade: Vibrant, game-inspired interface.
grunge: Worn, distressed look with bold textures.
elegant: Soft colors with smooth transitions.

To change the UI style, update Config.UIStyle in config.lua. For example:
Config.UIStyle = "cyberpunk"

Dependencies

qb-core: Required for core framework functionality.
qb-menu (optional): Enhances menu interactions.
qb-vehicleshop (optional): For vehicle purchase integration.

Usage

Access Garages: Approach a configured garage location and interact (default: E key).
Select Vehicle: Use the UI to browse and spawn stored vehicles.
Store Vehicle: Drive a vehicle to a garage and select the store option.
UI Customization: Admins can change the UI style via config.lua.

Support
For issues or feature requests, visit the GitHub Issues page or join our Discord for community support.
Contributing
Contributions are welcome! Fork the repository, make changes, and submit a pull request. Ensure code follows QBCore standards and includes documentation.
License
This project is licensed under the MIT License. See the LICENSE file for details.

