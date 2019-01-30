# Forensic-Browser

Online privacy is a highly researched area, with browser fingerprinting turning out to be a major area of concern. All the current defenses limit themselves to raising alerts when a JavaScript API with the potential to track the user is called. We are trying to modify an existing browser (Firefox) to log all the JavaScript code that is being loaded while a site is visited, and use the data for better analysis of the cause for tracking (if any) as well as better mitigation for the future. We also log attempts to canvas fingerprinting by emitting information on the caller script (like script name, line and column number) by modifying the toDataURL() and getImageData() methods in the browser's canvas library.

I worked with Firefox Nightly v65.01a for this project
