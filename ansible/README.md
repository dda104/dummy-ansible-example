# Dummy Example Using Ansible

1. Create and activate virtualenv

    ```shell
    ls .venv || python3 -m venv .venv
    [ -n VIRTUAL_ENV ] && source .venv/bin/activate
    ```

2. Install dependencies

    ```shell
    pip install -r requirements.txt
    ```

3. Install galaxy dependencies

    ```shell
    mkdir roles/
    ansible-galaxy role install -r requirements.yml -p roles/
    ansible-galaxy collection install -r requirements.yml
    ```

4. Run ansible playbook

    ```shell
    ansible-playbook playbook.yml
    ```
