# kube.mysql

# kube.wordp
echo "# kube.mysql" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:thlasta/kube.mysql.git
git push -u origin main


# Repo clonen
git clone git@github.com:thlasta/kube.mysql.git

# Repo auschecken/holen
git pull git@github.com:thlasta/kube.mysql.git

# Bei Änderungen:
git commit -m "Änderungsbeschreibung"
git push --all

# Jump one folder up, and apply to the whole folder:
kubectl apply -f mysql/

# Namespace "mysql" anlegen
kubectl create namespace mysql

