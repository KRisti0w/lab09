## Отчёт к lab09
В рамках выполнения данной лабораторной работы мною были выполнены все команды из `tutorial`:
1) Скопирован репозиторий из `lab08`.
2) Установлен `github-release`:
```bash
$ go install github.com/github-release/github-release@latest
go: downloading github.com/github-release/github-release v0.11.0
go: downloading github.com/dustin/go-humanize v1.0.1
go: downloading github.com/voxelbrain/goptions v0.0.0-20180630082107-58cddc247ea2
go: downloading github.com/kevinburke/rest v0.0.0-20250718180114-1a15e4f2364f
go: downloading github.com/tomnomnom/linkheader v0.0.0-20180905144013-02ca5825eb80
```
3) Установлен `GPG`
```bash
 $ sudo $PACKAGE_MANAGER install ${GPG_PACKAGE_NAME}
Обновление:
  dirmngr  gnupg  gnupg-l10n  gnupg-utils  gpg  gpg-agent  gpg-wks-client  gpgconf  gpgsm  gpgv

Сводка:
  Обновление: 10, Установка: 0, Удаление: 0, Пропуск обновления: 216
  Объём загрузки: 3 405 kB
  Требуемое пространство: 0 B / 11,1 GB доступно

Продолжить? [Д/н] Д
Пол:1 http://deb.debian.org/debian trixie/main amd64 gpgsm amd64 2.4.7-21+deb13u1+b3 [276 kB]
Пол:2 http://deb.debian.org/debian trixie/main amd64 gnupg-utils amd64 2.4.7-21+deb13u1+b3 [195 kB]
Пол:3 http://deb.debian.org/debian trixie/main amd64 gpg-wks-client amd64 2.4.7-21+deb13u1+b3 [109 kB]
Пол:4 http://deb.debian.org/debian trixie/main amd64 gpg amd64 2.4.7-21+deb13u1+b3 [635 kB]
Пол:5 http://deb.debian.org/debian trixie/main amd64 dirmngr amd64 2.4.7-21+deb13u1+b3 [384 kB]
Пол:6 http://deb.debian.org/debian trixie/main amd64 gnupg all 2.4.7-21+deb13u1 [417 kB]
Пол:7 http://deb.debian.org/debian trixie/main amd64 gpgconf amd64 2.4.7-21+deb13u1+b3 [129 kB]
Пол:8 http://deb.debian.org/debian trixie/main amd64 gpg-agent amd64 2.4.7-21+deb13u1+b3 [271 kB]
Пол:9 http://deb.debian.org/debian trixie/main amd64 gnupg-l10n all 2.4.7-21+deb13u1 [749 kB]
Пол:10 http://deb.debian.org/debian trixie/main amd64 gpgv amd64 2.4.7-21+deb13u1+b3 [241 kB]
Получено 3 405 kB за 0с (8 983 kB/s)
Чтение журналов изменений... Выполнено
(Чтение базы данных … на данный момент установлено 158877 файлов и каталогов.)
Подготовка к распаковке …/0-gpgsm_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается gpgsm (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Подготовка к распаковке …/1-gnupg-utils_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается gnupg-utils (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Подготовка к распаковке …/2-gpg-wks-client_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается gpg-wks-client (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Подготовка к распаковке …/3-gpg_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается gpg (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Подготовка к распаковке …/4-dirmngr_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается dirmngr (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Подготовка к распаковке …/5-gnupg_2.4.7-21+deb13u1_all.deb …
Распаковывается gnupg (2.4.7-21+deb13u1) на замену (2.4.7-21) …
Подготовка к распаковке …/6-gpgconf_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается gpgconf (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Подготовка к распаковке …/7-gpg-agent_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается gpg-agent (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Подготовка к распаковке …/8-gnupg-l10n_2.4.7-21+deb13u1_all.deb …
Распаковывается gnupg-l10n (2.4.7-21+deb13u1) на замену (2.4.7-21) …
Подготовка к распаковке …/9-gpgv_2.4.7-21+deb13u1+b3_amd64.deb …
Распаковывается gpgv (2.4.7-21+deb13u1+b3) на замену (2.4.7-21+b3) …
Настраивается пакет gnupg-l10n (2.4.7-21+deb13u1) …
Настраивается пакет gpgv (2.4.7-21+deb13u1+b3) …
Настраивается пакет gpgconf (2.4.7-21+deb13u1+b3) …
Настраивается пакет gpg (2.4.7-21+deb13u1+b3) …
Настраивается пакет gnupg-utils (2.4.7-21+deb13u1+b3) …
Настраивается пакет gpg-agent (2.4.7-21+deb13u1+b3) …
Настраивается пакет gpgsm (2.4.7-21+deb13u1+b3) …
Настраивается пакет dirmngr (2.4.7-21+deb13u1+b3) …
Настраивается пакет gnupg (2.4.7-21+deb13u1) …
Настраивается пакет gpg-wks-client (2.4.7-21+deb13u1+b3) …
Обрабатываются триггеры для man-db (2.13.1-1) …
Сканирование процессов...
Сканирование кандидатов...
Сканирование образов linux...

Запущено ядро последней версии.

Службы не требуют перезапуска.

Контейнеры не требуют перезапуска.

Сеансы пользователей с устаревшими процессами:
 kristina @ user service: gpg-agent.service[1225]

No VM guests are running outdated hypervisor (qemu) binaries on this host.
```
4) Сгенерирована пара ключей (мною были выбраны RSA И RSA)
```bash
$ gpg --batch --passphrase '' --quick-generate-key "Kristina <kristi0iw0@gmail.com>" rsa2048 default never
gpg: создан каталог '/home/kristina/.gnupg/openpgp-revocs.d'
gpg: сертификат отзыва записан в '/home/kristina/.gnupg/openpgp-revocs.d/B2E3342CA7F43267B8FCE5F5B6B4CC630DAFCF7C.rev'.
```
Результат:

```bash
$ gpg --list-secret-keys --keyid-format LONG
gpg: проверка таблицы доверия
gpg: marginals needed: 3  completes needed: 1  trust model: pgp
gpg: глубина: 0  достоверных:   1  подписанных:   0  доверие: 0-, 0q, 0n, 0m, 0f, 1u
/home/kristina/.gnupg/pubring.kbx
---------------------------------
sec   rsa2048/B6B4CC630DAFCF7C 2026-06-03 [SC]
      B2E3342CA7F43267B8FCE5F5B6B4CC630DAFCF7C
uid               [  абсолютно ] Kristina <kristi0iw0@gmail.com>
```

5) Получение ID ключа подписи и экспорт публичного ключа с последующим добавлением его на github:
```bash
$ GPG_KEY_ID=$(gpg --list-secret-keys --keyid-format LONG | grep ssb | tail -1 | awk '{print $2}' | awk -F'/' '{print $2}')
$ GPG_SEC_KEY_ID=$(gpg --list-secret-keys --keyid-format LONG | grep sec | tail -1 | awk '{print $2}' | awk -F'/' '{print $2}')
$ gpg --armor --export ${GPG_KEY_ID}
-----BEGIN PGP PUBLIC KEY BLOCK-----

mQENBGof+IABCADSuthWXE97pwj7ml4+upN7QcEbT7fWMP1aNXQEpoINLPYkNgQ/
h+cztvYKHdUadwATLgfyruTBKtdpRjv/CM6Xi15QEeJQoGPmPZGfh5LHCf9Jte89
1R8hqE71b//nacB7YELOaCfhvok/M5xmQzgJwl83Zlq/+CgiFcKeO44mnHxLBvso
tTSB5WiXfl174X3t2C/L78iu77LqmksdJQ/p3W2H/1OcR+v4kMIMlJxFz5ea8yBh
ZC+mrjHWjS9UdRwvVIPU29CWIPiWmUF9WXbyub//fkAfLYLXtBhAgDpeVqjy4TEV
FhHwB0RUZOx03E6joD2Xfv/gARFI93O9QAkRABEBAAG0H0tyaXN0aW5hIDxrcmlz
dGkwaXcwQGdtYWlsLmNvbT6JAU4EEwEKADgWIQSy4zQsp/QyZ7j85fW2tMxjDa/P
fAUCah/4gAIbAwULCQgHAgYVCgkICwIEFgIDAQIeAQIXgAAKCRC2tMxjDa/PfOB2
B/0UKK+7REIeXj4ylTaTT3v/BPeKAUH82FqtPilQhonVapcFONB7NBmewxTbmAJr
rOF6LdsrO+5bD1/khk41Cn3HYJTzEQsvE3+ik9xwp+NPjSLmwi2Uvlz9PebHkNhO
eEEgtd5Erfs5xCL+Y5jaGqTycBbgicB3VRWlJF0EDEzQo9uXgQv2BAxiP+9EETDz
+Dsi64/nT4QV/6XJX4h48QutEGi0wGvZKTt7nFXkymGOPZFTbBty1Q/59lzMdykF
l2mWHHXAOuAWxJbdGIqtVsNnEPatzhZdtTCBLFDEXf8jKfgnA1WENXoTR4A/BrGi
fPT4iuXzGJCWqe4geB/KIyld
=eloP
-----END PGP PUBLIC KEY BLOCK-----
```
Настройка Git для работы с GPG:
```bash
$ git config user.signingkey ${GPG_SEC_KEY_ID}
$ git config gpg.program gpg
```
Настройка переменной GPG_TTY 
```bash
$ test -r ~/.bash_profile && echo 'export GPG_TTY=$(tty)' >> ~/.bash_profile
$ echo 'export GPG_TTY=$(tty)' >> ~/.profile
```

6) Создан подписанный и верифицированный тег:
```bash
$ git tag -s v0.1.0.0 -m "v0.1.0.0 - first release"
$ git tag -v v0.1.0.0
object 536d01d9418084e87e1e5364f7f156538a3b55b7
type commit
tag v0.1.0.0
tagger Kristina <kristi0iw0@gmail.com> 1780480735 +0300

v0.1.0.0 - first release
gpg: Подпись сделана Ср 03 июн 2026 12:58:55 MSK
gpg:                ключом RSA с идентификатором B2E3342CA7F43267B8FCE5F5B6B4CC630DAFCF7C
gpg: Действительная подпись пользователя "Kristina <kristi0iw0@gmail.com>" [абсолютное]

$ git show v0.1.0.0
```
tag v0.1.0.0
Tagger: Kristina <kristi0iw0@gmail.com>
Date:   Wed Jun 3 12:58:55 2026 +0300

v0.1.0.0 - first release
-----BEGIN PGP SIGNATURE-----

iQEzBAABCgAdFiEEsuM0LKf0Mme4/OX1trTMYw2vz3wFAmof+t8ACgkQtrTMYw2v
z3xiewgAiQoAACNBwXGFCWaQtoNqjwCAc61mdGj4L8tce22AvEZEIkkwq3cZWpBD
kItATdvoknu0gu6iDmGOb0fZf0q1v0BdGyI5GYCobO70WUp+GPrP5wXmcLxzJBEB
JLXs0sqk0Kubg303hOltbnvfoEsNaJcmHoaYuD0nV5FciF5RDoVmSom4+WfpXL4R
uodQW3U9CkkByJHtL3bAix/qMd8kfrOUZdcf8x6oheYFkAFY+21C3GJmeGxM1YbD
RmdtJ9DFa9DqTICyxsmM0rI0Tv4sGeV6BdCKyYnEVUZT7U+J9nSHF173C7LMioQu
5MfDCLNbgFR4ihd8SAzF/XqKRlt2ZQ==
=HC72
-----END PGP SIGNATURE-----

commit 536d01d9418084e87e1e5364f7f156538a3b55b7 (HEAD -> main, tag: v0.1.0.0)
Author: KRisti0w <kristi0iw0@gmail.com>
Date:   Thu May 14 09:48:18 2026 +0300

    Update README.md

diff --git a/README.md b/README.md
index 57a5a7a..59fca8d 100644
--- a/README.md
+++ b/README.md
@@ -1,330 +1,178 @@
```
Тег запушен в репозиторий:
```bash
$ git push origin main --tags
Username for 'https://github.com': KRisti0w
Password for 'https://KRisti0w@github.com':
Перечисление объектов: 118, готово.
Подсчет объектов: 100% (118/118), готово.
При сжатии изменений используется до 2 потоков
Сжатие объектов: 100% (59/59), готово.
Запись объектов: 100% (118/118), 41.60 КиБ | 5.20 МиБ/с, готово.
Total 118 (delta 38), reused 117 (delta 38), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (38/38), done.
To https://github.com/KRisti0w/lab09
 * [new branch]      main -> main
 * [new tag]         v0.1.0.0 -> v0.1.0.0
```
8) Создан релиза, привязанный к тегу:
```bash
$ github-release info -u ${GITHUB_USERNAME} -r lab09
tags:
- v0.1.0.0 (commit: https://api.github.com/repos/KRisti0w/lab09/commits/536d01d9418084e87e1e5364f7f156538a3b55b7)
releases:
$ github-release release --user KRisti0w --repo lab09 --tag v0.1.0.0 --name "libprint" --description "my first release"
```
https://github.com/KRisti0w/lab09/releases/tag/v0.1.0.0

9) Cобранный архив загружен в релиз:
```bash
$ export PACKAGE_OS=`uname -s` PACKAGE_ARCH=`uname -m` 
$ export PACKAGE_FILENAME=print-${PACKAGE_OS}-${PACKAGE_ARCH}.tar.gz
$ github-release upload --user KRisti0w --repo lab09 --tag v0.1.0.0 --name "print-Linux-x86_64.tar.gz" --file print-Linux-x86_64.tar.gz
```

10) Проверям, что архив доступен для скачивания и содержит верные файлы:
```bash
$ github-release info -u ${GITHUB_USERNAME} -r lab09
tags:
- v0.1.0.0 (commit: https://api.github.com/repos/KRisti0w/lab09/commits/536d01d9418084e87e1e5364f7f156538a3b55b7)
releases:
- v0.1.0.0, name: 'libprint', description: 'my first release', id: 333628378, tagged: 03/06/2026 at 09:58, published: 03/06/2026 at 10:08, draft: ✗, prerelease: ✗
  - artifact: print-Linux-x86_64.tar.gz, downloads: 0, state: uploaded, type: application/octet-stream, size: 187 B, id: 437160239

$ wget https://github.com/${GITHUB_USERNAME}/lab09/releases/download/v0.1.0.0/${PACKAGE_FILENAME}
--2026-06-03 13:26:09--  https://github.com/KRisti0w/lab09/releases/download/v0.1.0.0/print-Linux-x86_64.tar.gz
Распознаётся github.com (github.com)… 140.82.121.4
Подключение к github.com (github.com)|140.82.121.4|:443... соединение установлено.
HTTP-запрос отправлен. Ожидание ответа… 302 Found
Адрес: https://release-assets.githubusercontent.com/github-production-release-asset/1257439487/4288c06d-6e59-40e8-905f-3e63861dd53a?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-06-03T11%3A18%3A49Z&rscd=attachment%3B+filename%3Dprint-Linux-x86_64.tar.gz&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-06-03T10%3A18%3A42Z&ske=2026-06-03T11%3A18%3A49Z&sks=b&skv=2018-11-09&sig=HPF7TvOP54PhYrC55hXx4hbLX%2BrlpIx2QeugCopEb3Y%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc4MDQ4MjY3MCwibmJmIjoxNzgwNDgyMzcwLCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.4TK4XfEw2bGhc26wHUZvHOm6UfTBuvpn0UWHbH8VsVU&response-content-disposition=attachment%3B%20filename%3Dprint-Linux-x86_64.tar.gz&response-content-type=application%2Foctet-stream [переход]
--2026-06-03 13:26:10--  https://release-assets.githubusercontent.com/github-production-release-asset/1257439487/4288c06d-6e59-40e8-905f-3e63861dd53a?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-06-03T11%3A18%3A49Z&rscd=attachment%3B+filename%3Dprint-Linux-x86_64.tar.gz&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-06-03T10%3A18%3A42Z&ske=2026-06-03T11%3A18%3A49Z&sks=b&skv=2018-11-09&sig=HPF7TvOP54PhYrC55hXx4hbLX%2BrlpIx2QeugCopEb3Y%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc4MDQ4MjY3MCwibmJmIjoxNzgwNDgyMzcwLCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.4TK4XfEw2bGhc26wHUZvHOm6UfTBuvpn0UWHbH8VsVU&response-content-disposition=attachment%3B%20filename%3Dprint-Linux-x86_64.tar.gz&response-content-type=application%2Foctet-stream
Распознаётся release-assets.githubusercontent.com (release-assets.githubusercontent.com)… 185.199.108.133, 185.199.109.133, 185.199.111.133, ...
Подключение к release-assets.githubusercontent.com (release-assets.githubusercontent.com)|185.199.108.133|:443... соединение установлено.
HTTP-запрос отправлен. Ожидание ответа… 200 OK
Длина: 187 [application/octet-stream]
Сохранение в: «print-Linux-x86_64.tar.gz.1»

print-Linux-x86_64.tar.gz.1   100%[=================================================>]     187  --.-KB/s    за 0s

2026-06-03 13:26:10 (521 KB/s) - «print-Linux-x86_64.tar.gz.1» сохранён [187/187]

$ tar -ztf ${PACKAGE_FILENAME}
release_files/
release_files/README.txt
```
