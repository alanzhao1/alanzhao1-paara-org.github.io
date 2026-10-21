# Previewing the site locally

## Prerequisites

The following packages are required on Ubuntu (other distros may differ):

```sh
sudo apt install build-essential ruby-dev
```

`ruby-dev` installs the Ruby headers for your distro's Ruby version (for example `ruby3.3-dev` on Ubuntu 25.04). `build-essential` is needed to compile native gem extensions.

## Usage

```sh
./preview.sh
```

Open http://localhost:4000. Jekyll auto-regenerates on file changes — just save and refresh.

Options are passed to `jekyll serve`. To check the site on a phone or tablet on the same network, run

```sh
./preview.sh --host 0.0.0.0
```

and open `http://<your computer's IP address>:4000` on the device.
