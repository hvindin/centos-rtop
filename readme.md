# rtop running on Centos7

This container contains rtop running on a Centos7 base.  

To run this container execute the following:  

        docker run -it --rm \ 
          -v $(dirname $SSH_AUTH_SOCK) \
          -e SSH_AUTH_SOCK=$SSH_AUTH_SOCK \
            hvindin/centos7-rtop user@host1.domain.com:22 user@host2.domain.com:22 user@host3.domain.com:22
