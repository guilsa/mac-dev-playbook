# Developer Checklist

This checklist outlines steps to take before and after running this Ansible script.

**Before running the script:**

- [ ] (Optional) Install [Oh My Zsh](https://ohmyz.sh/#install).
- [ ] Review [my dotfiles](https://github.com/guilsa/dotfiles/) dependency. Ansible will handle installation; manual cloning is not required.

**After running the script:**

- [ ] Open VSCode, enable Settings Sync, and [Backup and Sync Settings](https://code.visualstudio.com/docs/configure/settings-sync).

> **Note:** For testing in a macOS VM (via UTM), 32GB of disk space may be insufficient for Xcode installation. At least 64GB is recommended.

## Notes

I had to run `export PATH="$HOME/Library/Python/3.9/bin:/opt/homebrew/bin: $PATH"` otherwise when running the playbook with `ansible-playbook main.yml --ask-become-pass` I'd get `zsh: command not found: ansible-playbook`.
