#FROM quay.io/water-hole/ansible-operator
#FROM docker.io/djzager/ansible-operator:status-flag
FROM docker.io/djzager/ansible-operator:pr63

RUN ansible-galaxy install ansibleplaybookbundle.asb-modules

COPY . ${HOME}/roles/hello-world-apb
COPY playbooks ${HOME}/
COPY watches.yaml ${HOME}/watches.yaml
