---
# Selenium PAA
---
## Selenium Firefox Webdriver & PAA Script
``` Description

- Combines Selenium engine with the people_also_ask project based on bs4.
- Based on the Firefox Webdriver
- Removes requests modules and replaced with selenium

```

## Changelog (v1.5):
``` v1.5
- Added some functions into a class 'GSearch' (needs refined)
- Fixed RAM issues with webdriver not exiting properly (__init__, __del__)
- Removed selenium-wire integration (throwing HTTPS errors with new FF profile)
- Removed interceptor (selenium-wire)
- Adjusted default PAA scrape level to 7
- Tweak directory structure
```

### To-Do:
- [ ] Make clearer functions and better naming system
- [ ] Create function for taking SERP KWs > PAAs, and function for PAAs > Pickle/JSON
- [ ] Convert bash cleaning scripts to python and add to tools.py
- [x] Look into RAM handling/cleaning for performance (meantime pause/restart every 200 PAAs)
- [ ] Future: Use Click or similar module to allow running from the CLI 
- [ ] Add pickle to JSON converter to end of script
- [ ] Add command line arguments - e.g. for PROJECT_NAME, etc


### Requirements:
- requirements.txt
- Geckodriver =>0.31.0 https://github.com/mozilla/geckodriver/releases 
- Fill in local variables in constants.py file
- Filenames/structure work in progress - name files in input/output as per script
