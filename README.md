# Reject-Cases
This repository includes rejection cases by the App Store.


1- **DO NOT** use **App-Prefs** or **prefs:root** as these are __private API's__ like below
---------------------------------------------------------------------------------
  `UIApplication.shared.open(URL(string:"App-Prefs:root=General")!, options: [:], completionHandler: nil)`
  `[[UIApplication sharedApplication] openURL:[NSURL URLWithString:@"prefs:root=General"]];`
  
  Otherwise, [as mentioned this answer](https://stackoverflow.com/a/34024467/4711785) you might be get rejected.
