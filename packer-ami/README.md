# packer-ami-pbl-19

<!-- Packer installation on ubuntu -->

<!-- Add the HashiCorp GPG key. -->
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -

<!-- Add the official HashiCorp Linux repository. -->
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"

<!-- Update and install. -->
sudo apt-get update && sudo apt-get install packer

packer
Usage: packer [--version] [--help] <command> [<args>]

Available commands are:
    build           build image(s) from template
    console         creates a console for testing variable interpolation
    fix             fixes templates from old versions of packer
    fmt             Rewrites HCL2 config files to canonical format
    hcl2_upgrade    transform a JSON template into an HCL2 configuration
    init            Install missing plugins or upgrade plugins
    inspect         see components of a template
    validate        check that a template is valid
    version         Prints the Packer version