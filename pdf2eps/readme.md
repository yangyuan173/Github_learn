# To convert pdf to eps on Mac

- Install *homebrew*

      /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
- Install *poppler*

      brew install poppler
      
- Change permission of *pdf2eps*

      chmod 777 pdf2eps2
      
- Converting multiple files in *figure* folder

      for file in figure/*.pdf
      do
        ./pdf2eps $file
      done
