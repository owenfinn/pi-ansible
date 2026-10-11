# Pi bootstrap

    ansible-playbook site.yml -K          # -K if sudo needs a password
    ansible-playbook site.yml --check --diff   # dry run

Add a service: append an entry to `managed_services` in `group_vars/all.yml`.

Debug on the Pi:

    systemctl status reminder-printer
    journalctl -u reminder-printer -f
