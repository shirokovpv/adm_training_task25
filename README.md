# adm_training_task25
<h1 align="center">Занятие 25. Строим бонды и вланы</h1>
<h3 class="western"><span style="font-family: Roboto, serif;"><span style="font-size: small;">Описание задания</span></span></h3>
<p><span style="font-weight: 400;">в Office1 в тестовой подсети появляется сервера с доп интерфейсами и адресами</span></p>
<p><span style="font-weight: 400;">в internal сети testLAN:&nbsp;</span></p>
<p><span style="font-weight: 400;">- testClient1 - 10.10.10.254</span></p>
<p><span style="font-weight: 400;">- testClient2 - 10.10.10.254</span></p>
<p><span style="font-weight: 400;">- testServer1- 10.10.10.1&nbsp;</span></p>
<p><span style="font-weight: 400;">- testServer2- 10.10.10.1</span></p>
<p><span style="font-weight: 400;">Равести вланами:</span></p>
<p><span style="font-weight: 400;">testClient1 &lt;-&gt; testServer1</span></p>
<p><span style="font-weight: 400;">testClient2 &lt;-&gt; testServer2</span></p>
<p><span style="font-weight: 400;">Между centralRouter и inetRouter "пробросить" 2 линка (общая inernal сеть) и объединить их в бонд, проверить работу c отключением интерфейсов</span></p>
<h3 class="western"><a name="_heading=h.df570rpzx1qg"></a><span style="font-family: Roboto, serif;"><span style="font-size: small;">Используемые ОС</span></span></h3>
<p style="line-height: 108%; margin-bottom: 0.28cm;" align="justify"><span style="font-family: Roboto, serif;">Хостовая ОС Ubuntu 24.04 Desktop с установленным Vagrant 2.3.5. VirtualBox версия 7.0.26 r168464</span></span></p>
<h3 class="western"><span style="font-family: Roboto, serif;"><span style="font-size: small;">Выполнение</span></span></h3>
<p>******************************</p>
<p>Ввиду невозможности в нынешних реалиях воспользоваться стандартными репозиториями Vagrant (в РФ они сейчас не доступны), предложено обходное решение. Использован репозиторий, развернутый на&nbsp;<a href="https://vagrant.elab.pro/" rel="nofollow">https://vagrant.elab.pro/</a></p>
<p>Так как официальный пакет последней версии Vagrant также не доступен для скачивания, пакет взят оттуда же. Версия 2.3.5.</p>
<img width="411" height="88" alt="image" src="https://github.com/user-attachments/assets/7591c684-f543-4bf6-bfa8-3706a7648c97" />
<p>&nbsp;</p>
<p>Для подключения репозитория надо добавить в Vagrant-файл строку:</p>
<p><code>ENV['VAGRANT_SERVER_URL'] = 'https://vagrant.elab.pro'</code></p>
<p>И изменить box_name и box_version (как в репозитории, если туда зайти).</p>
<img width="254" height="135" alt="image" src="https://github.com/user-attachments/assets/5ad4ffb5-3949-4cd6-948b-d67050b86acc" />
<img width="238" height="274" alt="image" src="https://github.com/user-attachments/assets/aa6407df-e555-4e28-ac4f-7e8bb869c75c" />
<p>******************************</p>

