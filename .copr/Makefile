.PHONY: all srpm

all: srpm

srpm:
	dnf install -y rpmdevtools
	spectool -g ./slurm.spec
	rpmbuild -bs slurm.spec --define "_sourcedir $(PWD)" --define "_srcrpmdir $(outdir)"
