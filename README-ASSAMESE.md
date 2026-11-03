# Big Boss AI — Android APK project

এইটো Android APK build কৰিব পৰা project source। এই ZIP নিজে APK নহয়।

## GitHub-ত কেনেকৈ ব্যৱহাৰ কৰিব (Android ফোন)
1. GitHub-ত নতুন repository বনাওক: `BigBossAI-Android`.
2. ZIP extract কৰক আৰু project-ৰ ভিতৰৰ files/folders repository-ৰ root-ত upload কৰক (ZIP file অকল upload কৰিলে build নহ'ব).
3. এই project-ত GitHub Actions workflow ফাইল যোগ কৰক: `.github/workflows/build-apk.yml` (পৃথক build workflow template আপোনাক দিয়া হ'ব).
4. Actions tab-ত workflow run হ'লে `app-debug.apk` artifact হিচাপে পাব।

## বৰ্তমানৰ সীমাবদ্ধতা
- এই source-ত native Android WebView wrapper আৰু আগৰ Big Boss AI interface bundle কৰা হৈছে।
- AI screenshot analysis চলিবলৈ secure backend deploy কৰি frontend endpoint configure কৰিব লাগিব।
- Live market data provider সংযোগ কৰা হোৱা নাই। Quotex OTC feed বাহিৰৰ API-ৰ পৰা অনুমান কৰিব নোৱাৰি।
- CALL/PUT/NO TRADE কেৱল educational chart-condition output; লাভ নিশ্চিত নহয়।
- App-এ Quotex login, session/cookies বা auto-trading নকৰে।
- APK build successful হ'লেও backend/API setup নোহোৱালৈ AI/live data feature active নহ'ব।
