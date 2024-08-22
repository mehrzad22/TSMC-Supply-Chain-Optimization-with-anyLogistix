
## Overview

This project focuses on optimizing the distribution network of the Taiwan Semiconductor Manufacturing Company (TSMC). The main customers are located in China and the USA, with a factory in Taiwan and warehouses at key ports.

## Supply Chain Details

### Warehouses

- **Locations:** 
  - Tainan (Taiwan)
  - Hong Kong (China)
  - Long Beach (USA)

### Supply Policy

- Products shipped from the factory to Port Tainan.
- Products can be shipped between ports.
- Local warehouses only receive products from specified ports.
- Customers receive products from local warehouses.

### Costs

- **Operational Costs:**
  - Local Warehouse: $0.40/unit + $400 total
  - Port Warehouse: $0.24/unit + $700 total

- **Safety Stock:**
  - Local Warehouse: 10,000 units
  - Port Warehouse: 100,000 units

- **Penalties:**
  - Non-compliance: $50 million
  - Demand shortfall: $2.5/unit
  - Excess supply: $3/unit

### Transportation

#### Vehicles

| Vehicle Name        | Speed (km/h) | Capacity (thousand units) |
|---------------------|---------------------------|--------------|
| Cargo Ship          | 45                        | 800          |
| Truck               | 100                       | 5            |
| Full Size Carrier    | 90                        | 50           |

#### Cost Coefficients

| To               | From                | Cost Coefficient | Vehicle Type       | Direct Route? |
|--------------------|-------------------|------------------|---------------------|----------------|
| Local Warehouse     | Port              | 13.2             | Full Size Carrier    | No             |
| Local Warehouse     | Customer          | 14.5             | Full Size Carrier    | No             |
| Port                | Port              | 8.9              | Cargo Ship           | Yes            |
| Local Warehouse     | Customer          | 19.3             | Truck                | No             |
| Port                | Factory           | 10.6             | Full Size Carrier    | No             |

### Tariffs

- **Long Beach Port:** 25%
- **Hong Kong Port:** 34%

### Production Costs

- **Cost per Product:** $0.89
- **CO2 Emission Penalty:** $0.02
- **Selling Price:** $3.50

## The best routing
![image](https://github.com/user-attachments/assets/144cedb0-8754-4bff-b2a7-469151c1a172)

![image](https://github.com/user-attachments/assets/316175ee-7b83-4c0a-9a87-8f009a339de1)

![image](https://github.com/user-attachments/assets/149d84b3-87d1-4cbd-94b4-9ec04ba9b50a)





