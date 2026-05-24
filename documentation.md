# iBukas Energy
This project is a robust solar inverter management calculator system which will focus primarily on calculating load for a house hold and recommending the right type of system. The app will consist of various algorithm to help even the most basic of users get the best of experience.

## Predefined Appliances and Wattage
A json file containing a library of home appliances and a range of their wattage is provided; this will allow users to select all their appliances from a wide range of products, and also select the wattage for the product from our list or enter a wattage manually if they know it.

```
{
  "appliances": [
    {
      "id": 1,
      "name": "Bulb",
      "description": "A standard LED light bulb",
      "unit": "watts",
      "options": [10, 15]
    },

  ]
}
```

## Calculations
All the user-inputted appliances will be summed up to determine the total wattage required for the household. While not all appliances may run simultaneously, it's essential to include all devices that will be powered by the system to ensure sufficient capacity and prevent overloading.  

Let’s assume the total power requirement is **1,400W (1.4KW)**. To ensure the system can handle surge loads and efficiency losses, a **50% buffer** is added:  

**Required Inverter Size:**  
`1,400W × 1.5 = 2,100W (2.1KVA)` 
The Available Inverter rating for this is a `2.5KW 12V`

### Inverter Voltage Selection
The system voltage recommendation is based on the inverter size:

- If the inverter is **≤ 2.5KVA**, use a **12V system**.
- If the inverter is **between 2.5KVA and 5KVA**, use a **24V system**.
- If the inverter is **equal or above 5KVA**, use a **48V system**.

### Sunlight Hours Assumption
The average peak sunlight duration is assumed to be **5 hours per day** for solar energy calculations.


- ### How Long would you want your System to run on 1,400W?

Let's assume we want it to run for **5 hours**, the required energy would be:  
`1,400W × 5 hours = 7,000 WH` (approx **7kWh**)

- ### What would be the battery capacity?

We would be using a **48V system**, therefore:  
`7,000 WH ÷ 48V = 146 AH`  

To achieve this, we can use a **48V 150AH battery** (which provides **7.2kWh**). This would be enough to sustain the required 7kWh energy needed to run for **5 hours**.

- ### How Many Panels would be needed?

We are using **400W monocrystalline panels** and assuming **5 hours of peak sunlight**:

`Solar Panels Required = 7 kWh ÷ (400W × 5 hours) = 3.5` (approx **4 panels**)

So, we need **4 × 400W Solar Panels** (Total: **1,600W or 1.6kW**),  
a **minimum 2KVA inverter**, and  
**1 × 48V 150AH battery**.

## Summary of How Long This Will Run Your 1,400W Load
- **Daytime (Solar Only):** Panels produce **1,600W**, allowing you to run most appliances directly from solar during the day.  
- **Nighttime (Battery Only):** The **48V 150AH battery** stores **7.2kWh**, allowing for about **5 hours** of backup power for a **1,400W** load.

## Support & Sponsorship

Are you interested in using this **Solar Inverter Management Calculator** for your project?  
Would you like to **sponsor** its future development and improvements?

We welcome partnerships, sponsorships, and licensing opportunities.  
For inquiries, please contact us at **[your email or website]**.

