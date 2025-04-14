Steps to reproduce:

- Open a terminal within the project repo and run npm run build. This will start a new instance of your application in debug mode and will open a new window in the Excel Desktop app. You can close the Excel desktop window. Instead navigate to a workbook in Excel Online.
- Once you have a workbook open in excel online, navigate to "Add-ins" -> "Advanced" -> "Upload my Add-in" and navigate to the /manifest.xml file
- Once the manifest is loaded, you should see a "Get started with your sample add-in" notification.
- Click any cell and use the custom ADD function in the CONTOSO namespace by entering =CONTOSO.ADD(1, 2) (or any other combination of integers)
- Make sure this saves, close this window and clear your cache.
- Reopen this same workbook in Excel onilne and note that the custom function begins with _xldudf_
