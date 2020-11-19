# Ansible_Konfiguracija_NTP

1. Na sistem najprej namestimo Ansible

2. Potrebno je pripraviti hosts file v /etc/ansible (primer host fila je v mapi etc tega projekta). Upoštevati je potrebno tudi spremembo SSH porta (če imamo drugače kot default port 22). To spremembo lahko pri posameznem hostu nastavimo kot ansible_port=<številka porta>.

3. Celotno konfiguracijo iz mape Konfiguracija_NTP si skopiramo na strežnik.

4. Konfiguracijo nato poženemo znotraj mape z uporabo ukaza ansible-playbook konfiguracija_ntp.yml -u <uporabnisko ime> -k 
