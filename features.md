# LayerTrack — Features

LayerTrack is an offline-first poultry farm management app for Android. Everything runs on-device — no account required, no internet connection needed.

---

## Dashboard

The home screen gives you an at-a-glance view of your entire operation.

**Today's Summary**
- Total eggs collected today
- Actual revenue from sales recorded today
- Eggs sold, feed used (kg), and feed cost for the day
- *If all collected eggs were sold* estimate — shows projected revenue, cost, and profit based on your saved tray prices

**Last 7 Days Production Chart**
- Bar chart showing daily egg collection for the past week

**This Month**
- Eggs collected, revenue, and feed cost for the current calendar month
- Profit or loss figure with trend indicator

**All-Time Egg Sales**
- Total revenue, total feed cost, and net profit from all sales ever recorded
- Average selling price per egg

**Unsold Eggs — Potential Value**
- Running count of eggs collected but not yet sold, broken down by size (Small, Medium, Large, Extra Large)
- Set per-tray prices to see potential revenue, allocated feed cost, and potential profit
- Prices are saved and reused automatically

**Return on Investment (ROI)**
- Enter your startup capital once (housing, cages, birds, other expenses)
- Actual ROI %: `(all-time revenue − all-time feed cost − startup investment) ÷ startup investment × 100`
- Net profit after investment (positive = recovered + in profit, negative = still owed)
- Historical payback period based on your average monthly profit since day one
- Projected payback period based on your most recent 7-day daily profit rate — useful even on day one

**Flock Overview**
- Active flock count and total live bird count

**Quick Actions**
- One-tap shortcuts to Records, Flocks, Feed, and Sales

---

## Flocks

Track each group of birds separately through their entire lifecycle.

**Flock List**
- View all flocks or filter to active only
- Each card shows name, breed, current bird count, acquisition date, and active status

**Flock Detail**
- Full flock profile: name, breed, initial count, current count, acquisition date, notes
- Toggle active / inactive status at any time
- Event history with bird count impact shown per entry

**Add / Edit Flock**
- Name, breed/strain, initial bird count, acquisition date, notes

**Flock Events**
- Log anything that changes your flock — seven event types:
  - **Mortality** — birds that died (reduces count)
  - **Cull** — birds removed from production (reduces count)
  - **Bird Sale** — birds sold off (reduces count)
  - **Bird Purchase** — new birds added (increases count)
  - **Vaccination** — record vaccination dates (no count change)
  - **Medication** — record medication treatments (no count change)
  - **Other** — any other notable event
- Each event records the date, number of birds affected, and optional notes
- Current bird count updates automatically with each event

---

## Records

A three-tab calendar view covering production, feed consumption, and sales — all in one place.

### Production Tab

- Month-view calendar with each day highlighted when egg data exists for the selected flock
- Navigate backwards and forwards month by month
- Switch between your active flocks using the dropdown

**Day Detail**
- Tap any day to see all entries for that date
- Each entry shows the flock name, total sellable eggs, and a size breakdown: Small / Medium / Large / Extra Large
- Cracked egg count and daily mortality are shown when recorded
- Edit or delete any entry directly from the sheet

**Log Entry Form**
- Select flock and date (pre-filled from the tapped day)
- Enter count per size grade: Small, Medium, Large, Extra Large
- Optional cracked count and mortality count
- Live "sellable eggs" total updates as you type
- Notes field

### Feed Tab

- Calendar showing days when feed consumption was logged
- Available feed stock indicator at the top
- Tap any day to view, add, edit, or delete consumption entries for that date

**Feed Consumption Form**
- Select flock and date
- Choose feed per bird from preset amounts: 70g, 75g, 80g, 85g, 90g, 95g, 100g, 105g, 110g
- Total feed kg is calculated automatically based on your flock's current bird count
- Estimated cost is shown based on your most recent feed receipt price

### Sale Tab

- Calendar showing days when sales were recorded
- Tap any day to view, add, edit, or delete sale entries

**Sale Entry Form**
- Optional customer selection (or leave blank for walk-in)
- Per-size quantity and price fields: Small, Medium, Large, Extra Large
- Flexible pricing — set a different price per size per transaction
- Payment method: Cash, Transfer, Credit, Other
- Available egg inventory shown per size to avoid overselling
- Live revenue total preview
- Notes field

---

## Feed / Receipts

Track your feed supply from purchase through consumption.

**Inventory Summary**
- Current available feed stock in kg (purchased minus consumed)
- Stock status color indicator: normal, low (< 20 kg), or empty
- Estimated stock value based on most recent purchase price
- Total purchased, total consumed, and current price per kg

**Feed Receipts**
- Log every bag or batch of feed purchased
- Fields: date, feed type/brand, supplier, quantity (kg), total cost
- Cost per kg is calculated and stored automatically
- Edit or delete any receipt

**Feed Consumption**
- Separate from the Records screen — accessible here or from the Records Feed tab
- Full history of all consumption logs with flock, date, quantity, and estimated cost

---

## Sales / Customers

Manage the people you sell to and keep a full transaction history.

**Customer List**
- Filter active or all customers
- Each card shows name, phone, and address

**Customer Profile**
- Name, phone number, address, notes
- Active / inactive status
- Full transaction history for that customer

**Add / Edit Customer**
- Name, phone, address, notes, active status

**Sales Transactions**
- View today's sales or all sales across all time
- Each transaction shows: date, total revenue, total eggs, payment method, customer name, and a per-size breakdown
- Edit or delete any transaction

---

## Settings

**Appearance**
- Toggle between Dark Mode and Light Mode
- Change takes effect immediately and persists between sessions

**About**
- App version, developer contact, links to Privacy Policy, Terms of Service, FAQ, and the developer's website

---

## Onboarding

Shown once on first launch.

- **Theme selection** — choose Dark or Light mode before entering the app; live preview shows real app screenshots as you switch
- **Feature walkthrough** — five pages covering Production, Flocks, Feed, Sales, and Dashboard
- Skip to theme selection at any time
- Theme preference is saved and applied to the full app immediately

---

## Data & Privacy

- All data is stored locally on your device using a Room (SQLite) database
- No internet connection is required for any feature
- No account or sign-in is needed
- Nothing is transmitted to any server

---

## Egg Size Grades

LayerTrack uses four sellable size grades that match standard commercial classification:

| Grade | Label |
|---|---|
| Small | S |
| Medium | M |
| Large | L |
| Extra Large | XL |

Cracked eggs are tracked separately and excluded from sellable counts. A tray is 30 eggs.
