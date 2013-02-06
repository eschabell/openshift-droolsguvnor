Drools Guvnor on OpenShift
==========================
Installing the Guvnor component on OpenShift was never easier!

This git repository helps you get up and running quickly with the Guvnor component.


Running on OpenShift
--------------------

Create an account at http://openshift.redhat.com/

Create a jbossas-7.0 application

    rhc app create -a droolsguvnor -t jbossas-7 --from-code git://github.com/eschabell/openshift-droolsguvnor.git
    
That's it, you can now checkout your application at:

    http://droolguvnor-$your_domain.rhcloud.com/drools-guvnor

Note: there is no index.html for this project, only the above URL will work.

