# Web Scraping Assignment

## Overview
Web scraping is a technique for extracting information from websites. It involves making HTTP requests to a website's server, downloading the HTML content of the web page, and then parsing that HTML data to extract relevant information. The extracted data can be stored in a local file or database for further analysis or use.

I have performed web scraping to collect faculty member details from multiple FAST-NU campuses. The extracted data was then transformed into structured formats for further processing and analysis.

## Website Sources
Faculty data was collected from the following university websites:
- [Lahore Campus](http://lhr.nu.edu.pk/faculty/)
- [Islamabad Campus](http://isb.nu.edu.pk/Faculty/allfaculty/)
- [Karachi Campus](https://khi.nu.edu.pk/faculty-php/)
- [Chiniot-Faisalabad Campus](https://cfd.nu.edu.pk/all-departments/)
- [Peshawar Campus](http://pwr.nu.edu.pk/)

## Steps Performed
### **Step 1: Analyzing Website Structure**
- The faculty page structures varied across different campuses.
- Some campuses had a centralized faculty listing, while others had department-wise faculty pages.
- The necessary details were identified for extraction, ensuring consistency across all campuses.

### **Step 2: Data Extraction**
The following faculty details were extracted:
- **ID** (Integer)
- **Name** (String)
- **Designation** (String)
- **HEC Approved PhD Supervisor** (Boolean)
- **Highest Education** (String)
- **Email** (EMAIL)
- **Department** (String)
- **Extension** (Integer)
- **Image URL** (URL)

Each campus's data was stored in separate CSV files:
- `lhr.csv` (Lahore faculty data)
- `isb.csv` (Islamabad faculty data)
- `khi.csv` (Karachi faculty data)
- `cfd.csv` (Chiniot-Faisalabad faculty data)
- `pwr.csv` (Peshawar faculty data)

### **Step 3: Data Merging**
- All individual campus CSV files were concatenated into a single dataset.
- The final dataset was saved as `fast_faculty.csv`.

### **Step 4: Sampling Data**
- The last digit of my ID (3) was divided by 10 and used as the fraction value (0.3 / 30% ) for random sampling.
- A subset of the faculty data was extracted and saved as `sample.csv`.

## Deliverables
1. **Jupyter Notebook**: Includes well-documented Python code for web scraping and data processing.
2. **CSV Files**:
   - `lhr.csv`, `isb.csv`, `khi.csv`, `cfd.csv`, `pwr.csv` (campus-wise faculty data)
   - `fast_faculty.csv` (merged dataset)
   - `sample.csv` (randomly sampled data)
3. **ZIP Archive**: Contains all `.csv` files.


