# Renewable Energy System Simulator

### Project Scope
* Objective:
  * Create a tool to simulate the energy output of different renewable energy systems based on user inputs like location and system specifications
* End Users:
  * Potential users include students, researchers, project planners, or anyone interested in renewable energy
* Core Systems:
  * Solar power, wind power, hydroelectric power

### Research and Planning
* **Formulas:**
  * Solar Energy: 
    * To calculate the kWh produced by a solar panel, we need to know its wattage and the amount of sunlight it receives. Here's an example: Let's say you have a 300-watt solar panel 
      that receives an average of 5 hours of direct sunlight per day. To calculate the daily output in kWh, we would use the following formula:
    * Daily Output (kWh) = Wattage (W) x Hours of Sunlight x Efficiency
    * **Factors to consider**
      * The efficiency of a solar panel is how much of the energy it produces is converted into usable electricity. Most solar panels have an efficiency rating of between 15% and 20%.
      * The power rating of a solar panel, measured in watts (W), is a key factor in determining its energy generation potential. Solar panels with higher power ratings can produce 
        more electricity, making them an excellent choice for those looking to maximize their energy production
      * Consider the power rating of the solar panels you intend to purchase, as it will directly impact the maximum power output of your system.
      * Number of Solar Panels
      * Orientation of solar panels
      * Solar Panel Type and Quality

  * Wind Energy
    * P = 1/2pAv^3
      * p = Density  (kg/m3)  
      * A = Swept Area  (m2)  
      * v = Wind Speed  (m/s)  
      * P = Power 

  * Hydroelectric Energy
    * kinetic energy in flowing water starts out as gravitational potential energy. The gravitational potential energy of a given amount of water at any elevation can be calculated 
      using the following equation:
    * Pe = m x g x h
      * Pe = potential energy in Joules
      * m = the mass of the water in kg
      * g = the acceleration due to gravity (m/s2)
      * h = the height of the water in m (usually called the "head")
    * The force of gravity is essentially a constant (it gets a little bit smaller with height). Thus, all else being equal, as height and mass increase, the potential energy 
      increases. This equation only illustrates the maximum kinetic energy available to a hydropower system. In reality, there are always losses by the time the 
       kinetic energy is converted to electricity

* **Data Sources:**
  * Weather Data: 
    * Free weather api or visual crossing weather api
  * Geographic Data:
    * NASA power project maybe combined with OpenStreetMap (with SRTM data)
  * Energy System Specifications: make customizable 

### Dev Environment
* Programming Language: Python
* IDE: VS Code
* Version Control: Git repository
* Possible Libraries and Tools:
  * pandas (for data processing)
  * numpy (for calculations)
  * matplotlib or plotly (for visualization)
  * requests (for API calls)
  * Flask (for web development if applicable)
  * venv or conda (virtual environment)
  * Github for free domain - look into 

### System Architecture
* Backend Logic
  * Create classes or modules for each energy system (Solar, Wind, Hydro).
  * Each class should handle inputs (e.g., panel area, wind speed) and perform calculations based on the energy production formulas
  * Develop functions for fetching and processing weather and location data from APIs
* Frontend Design:
  * Web-based - sketch the layout using wireframes (tools like Figma can help).
  * Plan for input fields (e.g., location, system specs) and output displays (e.g., charts, tables).
* Data Flow:
  * User inputs location and system details.
  * System fetches relevant weather and geographic data.
  * Backend performs calculations based on the energy system selected.
  * Results are sent to the frontend for display.
