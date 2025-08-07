# 🔄 KOReader Progress Sync

Booklore enables you to synchronize your reading progress between KOReader and your Booklore library. You can push your current progress from KOReader to Booklore, or pull updates from Booklore back into KOReader to keep your reading status consistent across devices.

> ⚠️ **Note:**  
> Progress synchronization between the Booklore inbuilt reader and KOReader is **not supported** at this time, as they use different formats for storing reading progress.  
> Progress for KOReader and the inbuilt Booklore reader is maintained separately.

---

## 🛠️ Step 1: Configure KOReader Sync in Booklore

Before you can sync your reading progress, you need to enable and configure KOReader sync in your Booklore server. This involves setting up credentials and permissions for KOReader access.

![Booklore Device Settings](/img/koreader/1.jpg)

1. Go to **Settings** > **Device** in Booklore.
2. Click the **Edit** button to enable input fields for username and password.

---

![Booklore KOReader Credentials](/img/koreader/2.jpg)

3. Enter a username and a strong password for KOReader.
4. Click **Save** to store the credentials.
5. Toggle **Enable KOReader Sync** to activate syncing. You can disable it later if needed.
6. Copy the **API URL** shown, this will be required in KOReader.

---

![Booklore User Permissions](/img/koreader/3.jpg)

7. To allow users to access KOReader sync, assign them the **KOReader Sync** permission in **Settings** > **User**.
   - Only users with this permission can log in and sync their reading progress from KOReader.
   - If a user does not have the KOReader Sync role, Booklore will reject any sync attempts from KOReader for that user.
   - You can assign or remove this permission for each user individually, giving you control over who can use the sync feature.

---

## 📲 Step 2: Set Up Sync in KOReader

Once Booklore is configured, set up KOReader to connect to your Booklore server and begin syncing your reading progress.

![KOReader Settings](/img/koreader/5.jpg)

1. Open KOReader and go to **Settings** > **Progress Sync**.

---

![KOReader Custom Sync](/img/koreader/6.jpg)

2. Select **Custom Sync Server**.
3. Enter the API URL you copied from Booklore (e.g., `http://your-booklore-domain/api/koreader`).
4. Click OK to **Save**.

---

![KOReader Login](/img/koreader/7.jpg)

5. Select **Register / Login**.
6. Enter the username and password you set in Booklore.
7. Click **Login**.

---

![KOReader Push/Pull](/img/koreader/8.jpg)

8. To push your reading progress from KOReader to Booklore, select **Push progress from this device**.
9. To pull your reading progress from Booklore to KOReader, select **Pull progress from other devices now**.

---

![KOReader Matching](/img/koreader/9.jpg)
![KOReader Matching 2](/img/koreader/10.jpg)

10. Ensure the **Document matching method** is set to **Binary** for proper syncing.

---

![Booklore Synced Progress](/img/koreader/11.jpg)

- In Booklore, you can view synced progress on the book details page as a percentage and as a yellow progress bar under the cover.
- To reset progress, click **Reset Progress**. This only resets KOReader progress in Booklore; the device’s read status remains unchanged.

---

> 💡 **Tip:** If syncing fails, double-check your credentials, API URL, and network connection.
