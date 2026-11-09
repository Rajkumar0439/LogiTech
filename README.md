# Logistics Analytics Dataset

## Case Study Description
To analyze shipment reliability, warehouse efficiency, and inventory turnover in order to optimize logistics operations across regions.

---

## Dataset Overview
This dataset integrates shipment delivery logs, warehouse operations metrics, and inventory stock movement records to enable comprehensive analysis of logistics performance across multiple plants and regions.
---

### 1. `InventoryStockMovement` (2,036 records)
- **Purpose:** Tracks product‑level inventory status and stock movement across warehouses.  
- **Key Columns:**
  - `Product_ID` – Unique identifier for each product
  - `Warehouse_ID` – Plant/warehouse code
  - `Category` – Product category (Electronics, FMCG, Misc)
  - `Stock_On_Hand` – Current stock units available
  - `Reorder_Level` – Threshold level for triggering reorder
  - `Reorder_Flag` – Indicator if stock is below reorder level (1 = Yes, 0 = No)
  - `Avg_Lead_Time_Days` – Average supplier lead time in days
  - `Stockout_Days` – Number of days product faced stockout
  - `Carrying_Cost_Per_Unit` – Daily carrying cost per unit

---

### 2. `ShipmentDelivery` (209,402 records)
- **Purpose:** Captures shipment transactions, delivery timelines, and quality metrics.  
- **Key Columns:**
  - `Shipment_ID – Unique shipment identifier
  - `Customer – Customer code
  - `Warehouse_ID – Origin warehouse/plant
  - `Destination_Region – Delivery destination region/port
  - `Dispatch_Date – Date of shipment dispatch
  - `Delivery_Date – Date of delivery completion
  - `Delivery_Time_Days – Transit time in days
  - `Weight – Shipment weight in kg
  - `Carrier_Name – Logistics partner/carrier
  - `Shipment_Status – Delivery status (Delivered, Pending, etc.)
  - `Delivery_Mode – Mode of transport (Air, Road, etc.)
  - `Shipment_Cost – Cost of shipment
  - `Delivery_Accuracy_Flag – On‑time delivery indicator (1 = On‑time, 0 = Late)
  - `Damage_Flag – Damage indicator (1 = Damaged, 0 = Intact)  

---

### 3. `WarehouseOperation` (19 records)
- **Purpose:** Provides operational metrics for each warehouse facility.  
- **Key Columns:**
  - `Warehouse_ID – Unique warehouse/plant code
  - `Warehouse_Capacity_Units – Maximum storage capacity in units
  - `Current_Inventory_Units – Current stock units stored
  - `Inventory_Turnover_Ratio – Ratio of demand vs average inventory
  - `Order_Fulfilment_Rate – Percentage of orders fulfilled
  - `Avg_Pick_Pack_Time_Min – Average time to pick and pack orders
  - `Warehouse_Utilization_% – Utilization percentage of capacity
  - `Labour_Hours_Per_Day – Average labor hours per day
  - `Operational_Cost_Per_Day – Daily operational cost

---

##  Usage
This dataset is designed for:
- Shipment & delivery analytics → Route delays, on‑time delivery rates, cost per km benchmarking
- Warehouse efficiency analysis → Capacity utilization, labor productivity, pick‑pack time optimization
- Inventory management insights → Stockout frequency, reorder efficiency, turnover ratio across product categories
- Financial & operational evaluation → Cost per unit variation, procurement efficiency, budget allocation across warehouses and regions

---


