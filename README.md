Drools Guvnor on OpenShift
==========================
Installing the Guvnor component on OpenShift was never easier!

This git repository helps you get up and running quickly with the Guvnor component.


Running on OpenShift
--------------------

Create an account at http://openshift.redhat.com/

Create a jbossas-7.0 application

    rhc app create -a droolsguvnor -t jbossas-7

Add this upstream openshift-jbpmmigration repo

    cd droolsguvnor
    git remote add upstream -m master git://github.com/eschabell/openshift-droolsguvnor.git
    git pull -s recursive -X theirs upstream master
    # note that the git pull above can be used later to pull updates.
    
Then push the repo upstream

    git push

That's it, you can now checkout your application at:

    http://droolguvnor-$your_domain.rhcloud.com:8080/guvnor-webapp

