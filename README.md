# theoharti.github.io

This small site serves AdMob's mobile-app authorization file at
https://theoharti.github.io/app-ads.txt. The home page directs visitors to the
existing Depthworks support site; the support and privacy pages stay in
[TheoHarti/DepthworksSupport](https://github.com/TheoHarti/DepthworksSupport).

## Publish

1. In the repository's **Settings → Pages**, select **Deploy from a branch**,
   then **main** and **/(root)**, and save.
2. After deployment, open https://theoharti.github.io/app-ads.txt and confirm
   it returns the plain publisher line below, rather than an HTML page.

Future pushes to `main` update the published site automatically. The empty
`.nojekyll` file keeps these files static; `index.html` directs visitors to the
Depthworks support site.

```text
google.com, pub-2111037597422722, DIRECT, f08c47fec0942fa0
```

This repository holds the shared authorization file for FindusLab apps using
AdMob publisher `pub-2111037597422722`, including Depthworks on Android and iOS.
New apps using the same publisher and developer website can reuse this file.
Maintain the file here whenever authorized sellers change. Add separate seller
lines if other ad networks are introduced.

In Google Play, use https://theoharti.github.io/DepthworksSupport/ as the
developer website. In App Store Connect, use it as the marketing URL. Link the
published store entries in AdMob and request its app-ads.txt verification check.

See [Google's app-ads.txt setup instructions](https://support.google.com/admob/answer/9363762?hl=en)
and [GitHub Pages user site instructions](https://docs.github.com/en/pages/quickstart).
