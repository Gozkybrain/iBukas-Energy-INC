# iBukas Energy — Solar System Calculator

Plan your solar setup in minutes. Select your appliances, set your usage, and get instant estimates for inverters, batteries, and solar panels — no technical knowledge required.

**Try it live:** [ibukas-energy.netlify.app](https://ibukas-energy.netlify.app)

---

## How It Works

### 1. Add Your Appliances

Go to the [Calculator](https://ibukas-energy.netlify.app/calculator) page. A searchable dropdown lists 30+ common household appliances — fans, lights, TVs, fridges, ACs, laptops, water heaters, pumps, and more.

For each appliance:

- Choose **High** or **Low** wattage (based on typical ranges), or enter a **Custom** value if you know the exact rating.
- Set the **quantity** using the `−` / `+` stepper.
- Click **Add Appliance** to add it to your list.

![Calculator appliance selector](public/images/cost.webp)

### 2. Review Your List

The table shows every appliance you've added with its wattage, quantity, and subtotal. You can:

- **Edit** any row to adjust wattage or quantity inline.
- **Delete** items you don't need.
- See your **running total** in the sticky bar at the bottom.

### 3. Get Your Quote

Click **Get Complete Quote** to see your recommended system:

| What you'll see | Example |
|---|---|
| **Energy Required** | 7,000 Wh (1,400W × 5h) |
| **Recommended Inverter** | 2.5kVA — 12V system |
| **Battery Capacity Needed** | 146 Ah at 12V |
| **Solar Panels** | 4 × 400W panels (1,600W array) |
| **Battery Options** | 220Ah Tubular, 100Ah AGM, 200Ah Lithium — with unit counts |

You can adjust the load, hours, or inverter from the quote page and **Recalculate** on the fly.

---

## Use Cases

### Homeowner
You want backup power for lights, fans, a TV, and a fridge during outages. Add those appliances, see what inverter and battery you need, and how many solar panels to buy.

### Small Business Owner
You run a shop with freezers, lighting, and a cash register. Use the calculator to size a system that keeps you running through load-shedding.

### Solar Installer
Quickly generate a bill-of-materials for a client. Walk them through the calculator on-site, adjust parameters live, and export the quote.

### First-Time Solar Buyer
Not sure where to start? The step-by-step flow guides you from appliance selection to final system recommendation. No formulas, no guesswork.

---

## Pages

| Page | What it does |
|---|---|
| **Home** | Overview of services, partner brands, and what sets iBukas apart. |
| **Calculator** | Add appliances, set wattage/quantity, see total load. |
| **Quote** | Full system recommendation with inverter, battery, and solar panel estimates. |
| **Services** | Solar installation, inverter supply, maintenance, and free consultation. |
| **About** | How the calculator works, step-by-step guide, and why you can trust the numbers. |
| **Contact** | Email and social links for inquiries. |

---

## Built With

- **Next.js 15** — App Router, static generation
- **GSAP** — Scroll-triggered animations
- **CSS** — Custom styles, responsive breakpoints, no framework

---

## Local Development

```bash
npm install
npm run dev
```

The app runs at `http://localhost:3000`.

---

## Contact

- Email: [gozkybrain@gmail.com](mailto:gozkybrain@gmail.com)
- Twitter: [@gozkybrain4u](https://twitter.com/gozkybrain4u)

---

*iBukas Energy — Smart Solar for Your Home & Business*
