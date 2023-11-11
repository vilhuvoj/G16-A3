# Assignment 3 - Change
Group 16
## Description of the use case

The code begins by methodically scrutinizing the building model, where it categorizes materials into distinct categories, such as "Slabs" and "Walls," and proceeds to calculate their respective volumes. Following this, the code enhances the IFC model by incorporating material densities and corresponding CO2-equivalents per kilogram of material, sourced from a preexisting database stored in a Microsoft Excel file. Subsequently, the script computes the total weights of all elements and further derives CO2-equivalents for each element. These computed results are methodically structured, documented, and stored in an Excel file. This serves as a pivotal resource for conducting in-depth LCA analyses, allowing for a thorough assessment of the project's environmental impact and sustainability, with a primary focus on material utilization.

## Business value of the tool
- **Efficiency and Time Savings:** The tool streamlines the process of extracting material and environmental data from the BIM model, automating what would otherwise be a time-consuming and error-prone task. This increased efficiency can save significant time and resources for your company.
- **Data Accuracy:** By automating data extraction and calculations, the tool reduces the risk of manual errors and ensures the accuracy of the environmental impact assessments. This can be crucial for decision-making in construction projects and resource management.
- **Sustainability Compliance:** The tool supports your business in adhering to sustainability and environmental regulations. It helps in monitoring and managing the environmental impact of construction projects, which is essential for compliance and reputation management.
- **Competitive Advantage:** Demonstrating a commitment to sustainability and environmentally responsible practices can provide your business with a competitive edge. Clients and partners increasingly value environmentally conscious approaches, which can open up new opportunities and partnerships.

## Societal value of the tool
- **Environmental Impact Reduction:** By accurately quantifying the environmental impact of construction projects, the tool contributes to reducing the carbon footprint of the built environment. This benefits society by mitigating the negative effects of construction on the environment, such as, in this case, greenhouse gas emissions.
- **Transparency and Accountability:** The tool fosters transparency in construction projects by providing data on material usage and environmental impact. This transparency can lead to greater accountability in the construction industry, encouraging responsible practices.
- **Resource Conservation:** The tool promotes the efficient use of materials, which not only reduces waste but also contributes to the sustainable use of natural resources. This aligns with broader societal goals of resource conservation and sustainable development.

## Expertise used
To successfully solve the use case, following non-BIM disciplines and areas of expertise were involved:
- **Life Cycle Assessment (LCA)**
- **Programming (Python)**
- **Data Analysis and Processing**


## IFC concepts used
The code provided in the script utilizes various IFC concepts to interact with and extract information from the BIM model. These IFC concepts include:
- **IFC File Handling**: The code uses `ifcopenshell` library to open and manupulate IFC file.
- **IFC Entity Types**: The code filters and extracts specific IFC entity types, such as `IfcSlab` and `IfcWall`, to categorize and analyze elements based on their properties such as `IfcMaterial`.
- **IFC Property Sets**: The code accesses, extracts and also creates property sets associated with IFC elements. In this case, it retrieves material properties and volume information for slabs and walls and adds information about material denisities and kg of CO2-eq per kg of material.
> Note: Same approach might be conducted for other entities such as `IfcDoor`,`IfcWindow`,`IfcStair`,`IfcRoof` and more.

## Required disciplinary analysis
Analyzing the provided code and its broader context in a tool for LCA of a construction project involves following disciplinary analyses:
- **BIM and basic Construction Knowledge**: A basic understanding of BIM and construction practices is important to interpret and work with the data. This includes knowledge of architectural and engineering principles, as well as an understanding of how BIM data is structured and represented.
- **Life Cycle Assessment Expertise**: An in-depth knowledge of LCA principles and methodologies is central to conducting a thorough analysis of a building project's environmental footprint based on data provided by the script.
- **Excel and Spreadsheet skills**

## Important prerequisities for the use case
Before initiating this specific use, several prerequisite use cases or tasks must be completed. These preliminary steps include:
- **IFC File Preparation**: Preparing the IFC files to ensure they are structured correctly and conform to the industry-standard specifications is crucial. This might involve validating and cleaning the IFC data to remove errors and inconsistencies.
- **Python Environment**: Python is required to run the script. It can be downloaded from https://www.python.org/
- **Required Python Libraries**: It is necessary to have following Python libraries installed as the code is dependent on these libraries.
   - `ifcopenshell`: Can be installed using `pip install ifcopenshell`.
   - `openpyxl`: Can be installed using `pip install openpyxl`.
- **Microsoft Excel**: As the code exports results into Microsoft Excel worksheet, it is important to have it installed.
- **Database**: The code works with premade database of material densities and kg of CO2-eq per kg of material. It is necessary to create this database in advance.

## Other use cases revolving around the selected use case

The use case described can be a crucial component of larger, more comprehensive use cases in the fields of construction, sustainability, and project management. Here are some use cases that may benefit from the completion of this LCA analysis:

- **Sustainable Building Design:** The LCA results can inform architects and designers about the environmental impact of their design choices, helping them make sustainable decisions during the building design phase.

- **Construction Material Selection:** The LCA analysis can guide contractors and project managers in choosing construction materials that minimize environmental impact, reduce costs, and meet sustainability goals.

- **Green Building Certifications:** The LCA data can support the certification process for green building standards like LEED (Leadership in Energy and Environmental Design) and BREEAM (Building Research Establishment Environmental Assessment Method), providing evidence of sustainability practices.

- **Environmental Compliance:** The LCA analysis helps ensure that the construction project complies with environmental regulations and standards, minimizing the risk of non-compliance issues.

- **Project Funding and Investment:** For projects seeking investment or funding from sustainability-focused organizations or investors, the LCA results can be used to demonstrate the project's commitment to environmental responsibility.

- **Construction Project Documentation:** The LCA analysis can become a part of the project documentation, showcasing the project's environmental achievements and sustainability initiatives for future reference.

- **Environmental Impact Reporting:** In ongoing projects, regular LCA assessments can help in monitoring and reporting the evolving environmental impact and sustainability performance.

## Script explanation on an IDM diagram
![diagram](https://github.com/vilhuvoj/G6-A3/assets/150557585/0fdac90f-62f4-490d-9b91-f27b44153760)
