# 🧰 Toolkit
## This will be my toolkit.
### 🔍 curl and grep
```Bash
curl -sL mzelo.com | grep -iEC 5 browser|vpn|ip
``
* curl: The tool that "visits" the website and grabs the code.
   * -s (Silent): Keeps the terminal clean by hiding progress bars and
     download speeds.
   * -L (Location): Tells curl to "follow the move." If the site redirects
     (like from http to https), this flag ensures you get to the final
     destination.
Part 2: The Bridge (|)
   * | (The Pipe): This takes the wall of HTML code from curl and feeds it
     directly into the next command (grep) instead of letting it spill all
     over your screen.

Part 3: The Filter (grep -iEC 3)
   * grep: The tool that searches through text.
   * -i (Ignore Case): Finds "Browser", "browser", or "BROWSER" all the
     same.
   * -E (Extended): This is the "Magic Key" that allows you to use the |
     symbol inside your search to mean "OR".
   * -C 3 (Context): Shows you 3 lines above and 3 lines below every match.
     This is what lets you see the reasoning behind the word, not just the
     word itself.

  Part 4: The Target ("browser|vpn|ip")
   * "Quotes": The shield. It tells the shell: "Everything inside here is
     one single search pattern. Don't try to run 'vpn' as a program!"
   * browser|vpn|ip: Your "Red Flags." It searches for any of these three
     terms simultaneously.
