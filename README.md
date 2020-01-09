# Vuls Remote Scan

Run Vuls in a Docker container using Remote Scan Mode. This is just a docker-compose wrapper around the official tutorial https://vuls.io/docs/en/tutorial-docker.html to simplify using Remote Scan Mode.

## Usage

First you will need to retrieve various information (vulnerabilities, exploits and so-forth)

    # Fetch information for scanning Debian/Ubuntu/etc.
    docker-compose -f fetch-debian.yml up

    # Fetch information for scanning RedHat/CentOS/Fedora/etc.
    docker-compose -f fetch-redhat.yml up

Then you can run Remote Scan Mode

    docker-compose up
