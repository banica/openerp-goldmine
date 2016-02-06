ActivMail
=========

Script for migrating main partner data from Goldmine to OpenERP
---------------------------------------------------------------


**HOW TO USE IT:**

       1. Dependecies:
       
            A. pxtools package - you have it in *.tar.gz format

                tar xvf pxtools-0.0.20.tar.gz 
                cd pxtools-0.0.20/
                ./install-sh
                #  cc  or gcc compilers are needed, if don't exist on server:
                #          apt-get install gcc
                #          apt-get update
                #          apt-get upgrade
                #          apt-get install build-essential
                ./configure
                make
                make install

            B. openerplib python library - you have it in *.tar.gz format

                tar xvf openerp-client-lib.tar.gz
                cd openerp-client-lib
                python setup.py install

        2. Configuration

            At the beginning of the script at  # Parameters  section you can set: 
                database = <OpenERP database name where the data will be migrated>
                password = <The admin user password>
                pdox_folder = <relative path in filesystem from this script to paradox folder
                                with data to be migrated, e.g. ../home/calin/EXEMPLE >

        3. Run the script:

            >./gm_oerp def   # get default parameters from previous configuration or
            >./gm_oerp       # you have to introduce the data in interactive mode





