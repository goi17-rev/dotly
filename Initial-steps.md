## 🚀 Installation

Using wget:

```bash
bash <(wget -qO- https://raw.githubusercontent.com/CodelyTV/dotly/HEAD/installer)
```

Or using curl:

```bash
bash <(curl -s https://raw.githubusercontent.com/CodelyTV/dotly/HEAD/installer)
```

## 🐳 Try it in Docker

You can safely install additional software and make any changes to the file system. Once you exit zsh the image is
deleted.

<details>
<summary>Using Alpine:</summary>

```bash
docker run -e TERM -e COLORTERM -e LC_ALL=C.UTF-8 -w /root -it --rm alpine sh -uec '
  apk add curl sudo bash zsh git g++ python3
  bash -c "$(curl -fsSL https://raw.githubusercontent.com/CodelyTV/dotly/HEAD/installer)"
  zsh'
```
</details>

<details>
<summary>Or using Ubuntu:</summary>

```bash
docker run -e TERM -e COLORTERM -w /root -it --rm ubuntu sh -uec '
  apt-get update
  apt-get install -y curl build-essential sudo
  su -c bash -c "$(curl -fsSL https://raw.githubusercontent.com/CodelyTV/dotly/HEAD/installer)"
  su -c zsh'
```
</details>