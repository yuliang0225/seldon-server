SHEL=/bin/bash


test:
	nosetests -s -v seldon

bdist:
	python setup.py bdist_wheel --universal

sdist:
	python setup.py sdist

dist:sdist bdist

push:
	twine upload dist/*

clean:
	rm -rf build
	rm -rf dist
	rm -rf seldon.egg-info
