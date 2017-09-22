# Summary
goal is to provide some tools and structure to programmatically convert Github Markdown to PDF.

# Setup
Assumption made of Mac platform, with Homebrew.
Required packages: pandoc, mactex

```
brew update 
brew install pandoc
brew install ghc cabal-install
cabal user-config update
cabal install pandoc
## pandoc install took several minutes
brew cask install mactex
ln -s /Library/TeX/Root/bin/x86_64-darwin/pdflatex /usr/local/bin/pdflatex
```


# Usage
pandoc -o output/test.pdf test.md
