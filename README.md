# Angular-gtm
Google Tag Manager setup for Angular js
How to use Google Tag Manger to track Ajax site without using additonal pulgin.

#### Before start
1. Register your Google Tag Manager account by visiting http://tagmanager.google.com (Recommand V2)
2. Select or Create Acount and Container you wish to setup Tag

## Tracking Setup
- Page view
- Transaction (e-commerce tracking)

### Page View 
 
##### Add Variables (HistoryChange)
1. Select **Variables** from menu on the left.
2. Scroll to bottom **User-Defined Variable**, and add new Varibale by click **New** red color button.
3. 
  - Choose Type: **Auto-Event Varible**
  - Configure Variable: **History Change Source**
4. Click **Create Variable**
5. rename it's as **HistoryChange**

##### Add Triggers (Location Search)
1. Select **Triggers** from menu on the left, and add **New** Triggers
2. 
  Choose Event: **History Change**
  Fire On: **Some History Changes**
    - Select **HisotryChange** from the first dropdown
    - Select **does not contain** from second dropdown
    - Type in **replaceState** into last input field
3. Save the Trigger and label it as **Location Search**

##### Add Tags (GA - Page View)
1. Select **Tags** from menu on the left, and add **New** tag 
2.  - Choose Product: **Google Analytics**
    - Choose a Tag Type: `Depend of ur setup`
    - Configure Tag: 
      - tracking ID: **Your tracking ID**
      - Tracking type: **Page View**
    - Fire On: **`All Pages`**, **`Location Search`** (Click on More)
3. Create Tag
4. Lable it's as **GA - Page View**
  

