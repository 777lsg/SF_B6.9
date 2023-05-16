# SF_B6.9
1. Создайте Ansible-роль, настраивающую кэширующий DNS-сервер dnsmasq. Примените ее
- Роль deploy_dns
- Playbook play_dns.yml

2. Напишите Ansible-playbook, создающий группу пользователей superusers, куда входят пользователи user2 и user3, и которая, выполнив sudo -i, сможет повысить свои полномочия и стать root-пользователем. Можете использовать модуль lineinfile. У него есть параметр validate, позволяющий проверять сделанные изменения в файле. В документации есть пример валидации sudoers-файла.
- Роль deploy_sudo
- Playbook play_sudo.yml

3. Самостоятельно напишите Ansible-роль, настраивающую связку nginx+php-fpm и выдающую при обращении к главной странице веб-сервера информацию о php (содержимое index.php — <?php phpinfo();?>).
- Роль deploy_webs1
- Playbook play_webs1.yml

4. Дополните роль из п.3: пусть DocumentRoot будет в директории /opt/nginx/ansible. Используйте handler для перечитывания конфигурации nginx.
- Роль deploy_webs2
- Playbook play_webs1.yml