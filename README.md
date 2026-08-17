> # ⚠️ THIS VERSION IS DEPRECATED
>
> **This repository is no longer maintained and will not receive updates or bug fixes.**
>
> ### 👉 Get the new version here: **[jstdave.com/widgets](https://jstdave.com/widgets)**
>
> The new Overwatch Rank Widget — along with all my other widgets — is available on my website.
>
> The files in this repo are kept online for archival purposes only. If something breaks (API changes,
> new rank icons, season changes, etc.), it will **not** be fixed here.

---

# ℹ️ Important Information

This widget was solely made by me (JstDave). It would be nice if you could give me a follow or subscription on my Twitch channel at [https://twitch.tv/jstdave](https://twitch.tv/jstdave) if you like the widget!

If you need help or want to ask me something about the widget, please join the [Discord](https://dc.jstdave.com) or contact me on one of my [socials](https://jstdave.com/socials)!

---

# Overwatch 2 Rank Widget (Legacy / Deprecated)

This project **was** an Overwatch 2 Rank Widget that dynamically displays your current competitive ranks and divisions for all role categories (Damage, Tank, Support, and Open Queue). It includes smooth animations for rank changes and displays appropriate icons for each role.

**This standalone `Overlay.html` version has been replaced.** The current, actively developed version lives at **[jstdave.com/widgets](https://jstdave.com/widgets)**.

---

## Why switch to the new version?

- This is the actively maintained version — continued support, updates and bug fixes.
- Improved setup with more customization options.
- All my widgets in one place, with up-to-date instructions for each.

**➡️ [Go to jstdave.com/widgets](https://jstdave.com/widgets)**

---

## Migrating from this version

1. Head to **[jstdave.com/widgets](https://jstdave.com/widgets)** and grab the current version of the Overwatch 2 Rank Widget.
2. Follow the setup instructions there — you'll need the same details you used here (your BattleTag username and tag).
3. Point your existing OBS Browser Source at the new widget instead of the old one.
4. Done. You can delete the old `Overlay.html` folder.

---

<details>
<summary><b>📁 Legacy documentation (deprecated — click to expand)</b></summary>

> The instructions below apply to the **old, unsupported** version of the widget and are kept for reference only.
> Please use **[jstdave.com/widgets](https://jstdave.com/widgets)** instead.

## Features

- Real-time updates of Overwatch 2 competitive ranks for all roles.
- Smooth animations for rank changes with color indicators (green for rank up, red for rank down).
- Displays rank icons, division icons, and tier numbers for each role.
- Shows "NO RANK" for unranked categories.
- Customizable background image and player information.
- Easy integration into OBS as a local browser source.

---

## How to Use

### 1. **Download the Widget**

1. Click the green **Code** button at the top of the repository.
2. Select **Download ZIP** and extract the contents to a folder on your computer.

---

### 2. **Set Up Your Username and Tag**

1. Open the `Overlay.html` file in any text editor (e.g., Notepad, VSCode).
2. Locate the following section in the `<script>` tag:

    ```javascript
    // Put your information here
    const USERNAME  = "YOUR_USERNAME";  // Please put your username here
    const TAG       = "YOUR_TAG";       // Please put your tag here
    ```

3. Replace the placeholders with:
   - Your **Overwatch 2 username** (For example "JstDave" for the BattleTag "JstDave#2676").
   - Your **Overwatch 2 tag** (For example "2676" for the BattleTag "JstDave#2676").

---

### 3. **Change the Background Image**

1. Locate the `.rank-box` class in the `<style>` tag:

    ```css
    .rank-box {
        background-image: url('https://i.imgur.com/VW2vLbY.png');
    }
    ```

2. Replace the URL with the link to your preferred background image.
   - For example: `background-image: url('your-image-url-here');`

   Alternatively, you can use a local image by placing it in the same folder as `Overlay.html` and changing the URL to the file name.
   - Example: `background-image: url('background.jpg');`

---

### 4. **Add the Widget to OBS**

1. Open OBS Studio.
2. Add a new **Browser Source**.
3. Set the following:
   - **Local File:** Check the checkbox **"Local File"**.
   - **Browse:** Click the **Browse** button and select your `Overlay.html` file.
   - **Width:** 4400px (to accommodate all 4 role categories)
   - **Height:** 400px
4. Adjust the size and position of the widget in your OBS scene as needed.

---

## Role Categories

The widget displays ranks for all four competitive categories:

- **Damage** (DPS)
- **Tank**
- **Support**
- **Open Queue**

Each category shows the rank icon, division icon, and tier number (DIV 1-5) when ranked, or "NO RANK" when unranked.

---

## Notes

- The widget updates automatically every 2 minutes.
- Ensure your username and tag are correct to avoid errors.
- The widget uses the OverFast API which provides real-time Overwatch 2 data.
- Rank changes are animated with color coding (green for promotions, red for demotions).
- If you encounter issues, check the browser console for error messages. You can contact me on any social media ([My Socials](https://jstdave.com/socials))

---

## Example Picture

<img src="https://i.imgur.com/hsIGUj7.png" width="1200">

---

## API Information

This widget uses the [OverFast API](https://overfast-api.tekrop.fr/) to fetch Overwatch 2 competitive data. No API key is required, making setup simple and straightforward.

</details>

---

### 🔗 Links

- **New widget:** [jstdave.com/widgets](https://jstdave.com/widgets)
- **Twitch:** [twitch.tv/jstdave](https://twitch.tv/jstdave)
- **Discord:** [dc.jstdave.com](https://dc.jstdave.com)
- **Socials:** [jstdave.com/socials](https://jstdave.com/socials)
