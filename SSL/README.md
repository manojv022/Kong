

---

### ✅ Steps to Add SSL Certificate via Kong Manager (Portal)

#### 1. **Log in to Kong Manager**

* URL typically looks like: `http://<your-kong-host>:8002`
* You'll need an admin login.

#### 2. **Navigate to:**

`Certificates` → `Add Certificate`

#### 3. **Fill in the Certificate Details**

* **Certificate** – Paste the full certificate chain (including any intermediate certs).
* **Private Key** – Paste your `.key` file contents.
* **SNIs (Server Name Indication)** – Add one or more domain names this certificate will serve (e.g., `api.example.com`).

#### 4. **Click "Create" or "Save"**

That’s it — the certificate is now added and linked to the provided SNIs. Kong will serve that certificate when receiving TLS requests for those domains.

---

### 🔄 Updating a Certificate

Go to the `Certificates` list → click the **Edit** icon → replace the old cert/key → **Save**.

---

### 🔍 Notes:

* Kong does not serve certificates unless the SNI matches during a TLS handshake.
* If you're using **Route-level TLS** or **mutual TLS**, further config may be needed.
* You don’t need to restart Kong after adding or updating certificates — changes are live immediately.

---


