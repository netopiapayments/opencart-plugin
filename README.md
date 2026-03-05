# NETOPIA Payments – OpenCart Plugin

NETOPIA Payments (mobilPay) payment module for **OpenCart**, enabling **online card payments** on your store.

**Official documentation:** [OpenCart Plugin | NETOPIA Development Portal](https://doc.netopia-payments.com/docs/payment-plugins/opencart)

---

## Setting up

To set up the OpenCart plugin, follow these three steps:

### Step 1 – Create a Point of Sale

Make sure you have already created a **Point of Sale** configured for OpenCart. You will need the Point of Sale **signature** and **encryption/API keys** for the next steps.

- **Docs:** [Points of Sale](https://doc.netopia-payments.com/docs/get-started/point-of-sale)  
- **Merchant admin:** [https://admin.netopia-payments.com](https://admin.netopia-payments.com)

### Step 2 – Install and activate the plugin

1. Download the module from this repository (e.g. **Code → Download ZIP**).
2. Unzip the file. Select the **`install.json`** file and the **`admin`** and **`catalog`** folders, then compress them into a new `.zip`.
3. Rename the new archive to **`mobilpay.ocmod.zip`**.
4. In your OpenCart admin: **Extensions → Installer**. Click the upload button and upload **`mobilpay.ocmod.zip`**.
5. In **Installed Extensions**, find **NETOPIA Payments** and click the green **Install** button.
6. Go to **Extensions → Extensions**. Filter by **Payments**. Find **NETOPIA Payments** and click **Install** again to complete activation.

### Step 3 – Configure and validate

1. After installation, click the blue **Configure** (edit) button for NETOPIA Payments.
2. Fill in:
   - **Account Signature**  
   - **Live API Key**  
   - **Sandbox API Key**
3. **Account Signature:**  
   [admin.netopia-payments.com](https://admin.netopia-payments.com) → **Points of Sale** → **Options** (⋮) → **Technical Settings**.
4. **Live API Key:**  
   In the same dashboard: click your **profile image** (top right) → **Securitate** → enter a name (e.g. `opencart`) → **GENEREAZA CHEIE** → copy the new key and paste it into the **Live API Key** field in OpenCart.
5. **Sandbox API Key:**  
   In the Netopia dashboard, open **Mediu de testare** (test environment) in the left menu, then repeat the same API key generation steps and paste the key into the **Sandbox API Key** field in OpenCart.

After this, the technical integration is complete.

**Final step:** send an email to **[implementare@netopia.ro](mailto:implementare@netopia.ro)** to request final validation. The NETOPIA technical team will activate your Point of Sale so you can start accepting payments.

---

## Documentation and compatibility

- **Full guide (OpenCart 4 / API V2):**  
  [https://doc.netopia-payments.com/docs/payment-plugins/opencart](https://doc.netopia-payments.com/docs/payment-plugins/opencart)
- **Point of Sale setup:**  
  [https://doc.netopia-payments.com/docs/get-started/point-of-sale](https://doc.netopia-payments.com/docs/get-started/point-of-sale)
- **NETOPIA Payments:** [https://www.mobilpay.ro](https://netopia-payments.com/)

The NETOPIA Payments team aims to keep the module compatible with the latest OpenCart versions. For **older OpenCart versions** (e.g. 3.x), check other branches of this repository.

- Tested up to **OpenCart v3.0.3.8** (3.x branch)  
- Tested up to **PHP 8.0.x**
