
<!DOCTYPE html>
<!--[if lt IE 9 ]> <html class="ie8"> <![endif]-->
<!--[if IE 9 ]> <html class="ie9"> <![endif]-->
<!--[if (gt IE 9)|!(IE)]><!--> <html> <!--<![endif]-->
    <head>
        <meta charset="UTF-8" />

        <meta http-equiv="x-ua-compatible" content="ie=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">

        <title>Scratch - Imagine, Program, Share</title>

        <!-- Prevent mobile Safari from making phone numbers -->
        <meta name="format-detection" content="telephone=no">

        <!-- Search & Open Graph-->
        <meta name="description" content="Scratch is a free programming language and online community where you can create your own interactive stories, games, and animations." />
        <meta name="google-site-verification" content="m_3TAXDreGTFyoYnEmU9mcKB4Xtw5mw6yRkuJtXRKxM" />

        <meta property="og:url" content="https://scratch.mit.edu/" />
        <meta property="og:type" content="website" />
        <meta property="og:title" content="Scratch - Imagine, Program, Share" />
        <meta property="og:description" content="Scratch is a free programming language and online community where you can create your own interactive stories, games, and animations." />
        <meta property="og:image" content="https://scratch.mit.edu/images/scratch-og.png" />
        <meta property="og:image:type" content="image/png" />
        <meta property="og:image:width" content="986" />
        <meta property="og:image:height" content="860" />

        <!-- Favicon & CSS normalize -->
        <link rel="shortcut icon" href="/favicon.ico" />
        <link rel="stylesheet" href="/css/lib/normalize.min.css" />

        <!-- Polyfills -->
        <script src="/js/polyfill.min.js"></script>

        <!-- Analytics (GA) -->
        <script>
            /* eslint-disable */
            (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
            (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
            m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
            })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

            ga('create', 'UA-30688952-1', {
                'sampleRate': 10
            });
            ga('send', 'pageview');
            /* eslint-enable */
        </script>
    </head>

    <body>
        <div id="app"></div>

        <!-- Vendor & Initialize (Session & Localization)-->
        <script src="/js/common.bundle.js"></script>

        <!-- Scripts -->
        <script src="/js/splash.intl.js"></script>
        <script src="/js/splash.bundle.js"></script>

        <!-- Translate title element -->
        <script>
            var loc = window._locale || 'en';
            if (typeof window._messages !== 'undefined' && loc !== 'en') {
                if (typeof window._messages[loc] === 'undefined') {
                    loc = loc.split('-')[0];
                }
                if (typeof window._messages[loc] !== 'undefined') {
                    var localizedTitle = window._messages[loc]['general.' + 'Imagine, Program, Share'.toLowerCase()] || '';
                    if (localizedTitle.length > 0) {
                        document.title = 'Scratch - ' + localizedTitle;
                    }
                }
            }
        </script>
    </body>
</html>

