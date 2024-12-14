# Production instructions

This folder contains all the production files and a complete parts list necessary for manufacturing this board. The board includes both SMD and through-hole components. The PCB and SMD production files are optimized for ordering from JLCPCB, while the through-hole components are configured for ordering from Mouser.

## PCB

Upload the file `./jlcpcb/steiner-parker-vcf.zip` on [jlcpcb.com](https://www.jlcpcb.com) to order the PCB.

## SMD assembly

On JLCPCB, select the "PCB Assembly" option. Make sure you check:

- PCBA Type: Economic
- Assembly Side: Top Side
- PCBA Qty (up to you)
- Tooling Holes: Added by Customer
- Confirm Parts Placement: Yes
- Parts Selection: By Customer

Then hit Next.

Use the `./jlcpcb/bom.csv` (BOM) and `./jlcpcb/positions.csv` (CPL — position) files respectively to order SMD assembly by JLCPCB.

> Note: the BOM file contains _all_ parts (including through holes too), so you _will_ get a warning after uploading it. You can ignore this warning and continue with ordering.

![CleanShot 2024-12-14 at 11 21 11@2x](https://github.com/user-attachments/assets/68c7c8e5-fbf6-4e3e-9f3f-8e7e793af92d)

‼️ **Make sure you triplecheck the rotation of each SMD component with a dedicated pin order!**

![CleanShot 2024-12-14 at 11 21 53@2x](https://github.com/user-attachments/assets/d599f383-cb44-4a01-b2ea-aea06f3712b0)

## Through hole assembly

Well you guessed it: you'll need to solder all THT components yourself. It's fun, trust me, just make sure you don't smell the smoke from your soldering iron.

To make ordering through hole components easy we've prepared a CSV file to generate a BOM on [mouser.com](https://www.mouser.com). Here's what you need to do:

1. Go to [https://www.mouser.com](https://www.mouser.com) and log in with your account
2. Open [BOMs](https://hu.mouser.com/OrderHistory/Boms) from the account menu
3. Click on Create New BOM
4. Upload the `./mouser/steiner-parker-vcf-mouser-bom.csv` file from this directory
5. Make sure you map the `Quantity 1` and `Mouser Product Number` columns correctly
6. Create the BOM

You can order all necessary parts at once. If a part is not available you need to find replacement components, or if you want another vendor (like Digikey) then you'll need to hunt all parts yourself.

## Full BOM

The `./steiner-parker-vcf-full-bom.csv` file contains all the parts including SMD and through hole if anyone would need it.

## Disclaimer

We are not responsible for any errors in the PCB design or the parts list. All responsibility for ordering PCBs, components, and assembly services rests solely with you.

## More important disclaimer

Have fun!
