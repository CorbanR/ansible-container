default: core

core_exists=$(shell docker images | grep -c 'instructure-core')

#Default building ruby 2.3 image
ruby_version = 2.3

#Check to see if the core image has been build
#If not, build it. This wont really be an issue when
#ansible-container actually supports custom image tags.
check:
	if [ "$(core_exists)" == "0" ] ; then \
		ansible-container build --service core ; \
	fi

core:
	ansible-container build --service core

ruby: check
	ansible-container build --service ruby$(ruby_version)

all: check
	ansible-container build
