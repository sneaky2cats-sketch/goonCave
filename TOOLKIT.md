🧰 Toolkit
This will be my toolkit.
🔍 curl & grep
bash
Run

curl -sL mzelo.com | grep -iEC 5 browser|vpn|ip

    curl → Visits site & fetches code
        -s = Silent (clean output)
        -L = Follow redirects
    grep → Searches text
        -i = Ignore case
        -E = Extended patterns
        -C 5 = Show ±5 lines around match
        browser|vpn|ip = Keywords to find

    📌 Legend: curl [options] [url] | grep [options] [terms]
