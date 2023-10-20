# Getting started on the MEB UKB Uppmax project

TODO: introductory paragraph

## Joining the project

1. Follow the process to join at
    https://www.uppmax.uu.se/support/getting-started/applying-for-a-user-account/.
    First step is to register at [SUPR](https://supr.naiss.se/) using SWAMID (KI
    login) (or verify that you already have an account)

    If you know that you already have an account at SUPR, just go to the next
    step.

2. Request to join the project [Molecular epidemiologic studies of aging and
      age-related
      diseases](https://supr.naiss.se/project/request/?search=sens2017519)

## Connecting

3. Follow instructions for connecting to and using the Bianca cluster at
    https://www.uppmax.uu.se/support/user-guides/bianca-user-guide/. You will
    need to set up two-factor authentication for Uppmax (note that this is
    independent of any 2FA you may have for SUPR or KI).

    Access is possible using SSH in a terminal or PuTTY to connect to
    `<username>-sens2017519@bianca.uppmax.uu.se`, or through a graphical
    interface in your web browser at http://bianca.uppmax.uu.se/

    For getting data on and off the bianca cluster, you must use SFTP and
    connect to `sftp://<username>-sens2017519@bianca-sftp.uppmax.uu.se`.

The UKB genotype data is located in `/proj/sens2017519/nobackup`. See
[ukb_data_on_uppmax.md](ukb_data_on_uppmax.md) for detailed description of data locations and
guidelines for use.

