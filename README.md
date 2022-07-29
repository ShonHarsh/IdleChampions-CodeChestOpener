![](https://shonharsh.github.io/curriculum-vitae/images/idle-champions-logo.jpg)

# IdleChampions-CodeChestOpener
This project takes codes from a spreadsheet and opens chests in the game Idle Champions

### Getting Started

After making a pull request or downloading the project, open the Main.xaml in UiPath Studio.  The robot can be run with the play button in the ribbon and the result can be seen in output pane.

### Details

1. Clear the 'redeemed' status 'True' values in the spreadsheet ..\IdleChampions-CodeChestOpener\Data\Codes.xlsx.

2. In the Main.xaml, validate the strFilePath and the strSheetName variables in the Sequence Initializations sequence.  They should not need changed unless you moved the code file or changed the name of the sheet.

3. Important, in the game Idle Champion, the screen should be at the inventory screen just before clicking on a chest.

4. Codes that unlock heroes or achievements can break the program.  The screen recognition may not be able to succeed with the images that appear from these.

5. If an error is thrown the log will display codes that were processed.  Thus you can determine and smite the code caused the error.

### Sample Output

```
07/28/2022 21:24:02 => [Debug] Debug started for file: Main
07/28/2022 21:24:04 => [Info] IdleChampions-CodeChestOpener execution started
07/28/2022 21:24:05 => [Debug] IdleChampions-CodeChestOpener.Main.Begin;
07/28/2022 21:24:05 => [Debug] IdleChampions-CodeChestOpener.ReadCodes.Begin;
07/28/2022 21:24:06 => [Debug] IdleChampions-CodeChestOpener.ReadCodes.TryCatch; Codes read successfully.
07/28/2022 21:24:06 => [Debug] IdleChampions-CodeChestOpener.ReadCodes.End;
07/28/2022 21:24:06 => [Debug] IdleChampions-CodeChestOpener.IdleChampionsController.Begin;
07/28/2022 21:24:07 => [Debug] Audit: Using Desktop App. App: C:\\Program Files\\Epic Games\\IdleChampions\\idledragons.exe Arguments:
07/28/2022 21:24:12 => [Debug] IdleChampions-CodeChestOpener.IdleChampionsController.Part01.End;
07/28/2022 21:24:17 => [Debug] IdleChampions-CodeChestOpener.IdleChampionsController.Part02.isWindowOfferExpired; isWindowOfferExpired Match Case
07/28/2022 21:24:21 => [Debug] IdleChampions-CodeChestOpener.IdleChampionsController.Part02.End;
07/28/2022 21:24:22 => [Debug] IdleChampions-CodeChestOpener.IdleChampionsController.CodeNotRedeemed; Code Not Redeemed: YOUR-GUID-ETOD-ANDD
07/28/2022 21:24:22 => [Debug] IdleChampions-CodeChestOpener.IdleChampionsController.End;
07/28/2022 21:24:23 => [Info] IdleChampions-CodeChestOpener.Main.ForEach; Codes redemption operation completed.
07/28/2022 21:24:23 => [Debug] IdleChampions-CodeChestOpener.UpdateDataFile.Begin;
07/28/2022 21:24:27 => [Info] Audit: Using Excel File: C:\Cloud\Dropbox\Code\Robotic Process Automation\Projects\Personal\IdleChampions-CodeChestOpener\Data\Codes.xlsx
07/28/2022 21:24:29 => [Debug] IdleChampions-CodeChestOpener.UpdateDataFile.End;
07/28/2022 21:24:29 => [Debug] IdleChampions-CodeChestOpener.Main.End;
07/28/2022 21:24:29 => [Info] IdleChampions-CodeChestOpener execution ended in: 00:00:25
```

### Project Development Information
Studio 2022.4.3 - 5/27/2022
Community License
Per-user Installation

License Provider: Orchestrator
Activation ID:

Update Channel: Stable

Microsoft Windows 10 Pro 64-bit
6.0.2

### Requirements

[UiPath Studio](https://www.uipath.com/product/studio) is required to run the robot.

### Git Notes

Clone the project to develop or change it.

`git clone https://github.com/ShonHarsh/IdleChampions-CodeChestOpener`

### Links

[UiPath: Automation Platform](https://www.uipath.com/)

[UiPath Studio](https://www.uipath.com/product/studio)

[My Website](https://shonharsh.github.io/curriculum-vitae/index.html) - Errors, spelling fixes and comments are very welcome!
