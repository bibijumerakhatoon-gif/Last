Device Info Pro by @rk_badsha1435 - GitHub-ready project
=====================================================

यह पैकेज GitHub पर सीधा अपलोड करने के लिए तैयार किया गया है।
GitHub Actions workflow पहले से जुड़ा हुआ है — जिससे आप push करते ही APK बन जाएगा और Actions केArtifacts में मिलेगा।

बुनियादी निर्देश (एक बार):

1) GitHub पर नया रिपोजिटरी बनाइए (उदा: device-info-pro)
2) इस पूरी फोल्डर की सामग्री उस repo के root में upload (Add files → Upload files) कर दीजिए और Commit कर दीजिए
   - या लोकल से git push कर सकते हो (यदि git जानते हो):
     git init
     git add .
     git commit -m "initial commit"
     git branch -M main
     git remote add origin https://github.com/your-user/device-info-pro.git
     git push -u origin main

3) GitHub → Actions टैब पर जाइए। "Android CI - Build APK" workflow चालायें या simply push करें।
4) Build होने पर workflow run में नीचे "Artifacts" दिखाई देगा — वहां से `app-debug-apk` डाउनलोड करें।
5) डाउनलोड की हुई APK को अपने फोन पर install करिए (Settings → allow install from unknown sources यदि जरुरत हो)।

ध्यान दें:
- यह debug APK है — प्ले स्टोर पर डालने के लिए release signing की आवश्यकता होगी।
- अगर build fail हो तो Actions log copy करके मुझे दे दो, मैं help कर दूँगा।
