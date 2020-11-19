# Ansible_Konfiguracija_NTP

1. Na sistem najprej namestimo Ansible

2. Potrebno je pripraviti hosts file v <b>/etc/ansible</b> (primer host fila je v mapi etc tega projekta). Upoštevati je potrebno tudi spremembo SSH porta (če imamo drugače kot default port 22). To spremembo lahko pri posameznem hostu nastavimo kot <b>ansible_port=<številka porta></b>.

3. Celotno konfiguracijo iz mape <b>Konfiguracija_NTP</b> si skopiramo na strežnik.

4. Konfiguracijo nato poženemo znotraj mape z uporabo ukaza <b>ansible-playbook konfiguracija_ntp.yml -u <uporabnisko ime> -k</b>
  
5. Delovanje konfiguracije lahko nato preverimo z ukazom <b>chronyc sources</b>.
