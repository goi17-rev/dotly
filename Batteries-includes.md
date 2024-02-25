- ##dot command
    - Running `dot` will display all available global scripts
        - Personal scripts should be located in `<DOTFILES_PATH>/scripts`
        - Opinionated scripts are located `<DOTFILES_PATH>/modules/dotly/scripts`
    - Most useful dot scripts
        - symlinks apply: Applies all your new/updated symlinks
        - mac defaults: With this script you can import/export all your current Mac settings. After you run the import script, you'll need 
                        to restart your machine.
        - Press `<Ctrl-c>` once/twice to quit `dot`
- ##Updating dotly
   - git submodule update --init --recursive modules/dotly
- ##Shortcuts
   - If you press `<Ctrl-r>`, you'll get a custom reverse-search UI
- ##Opinionated dotfiles template
    - By default dotly came with a default template ready to use
      ```
      dotfiles/
          bin/
          doc/
          editors/
          git/
          langs/
          os/
          restoration_scripts/
          scripts/
          shell/
          symlinks/
      ```
      this does not mean that you can not modify this defaults, you can create/erase/rename everything. Just remember that you need to 
      update your symlinks in case you need it.