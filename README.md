_**Q1:**_


To run the manifests, command is given below

**kubectl apply -f automatanode.yml -f chaindata-pv.yml -f chaindata-pvc.yml**


I have created the persistent Volume and claim storage to store the data in case pod getting down so that data remains persistence! So, I have created the **static provisioning** to make data persistence and for Volume persistence already and EBS deployed on AWS by volume-ID: '**vol-082c078e9273325d3**' as mentioned in **chaindata-pv.yml**

And to claim that persistence Volume, created a fle name **chaindata-pvc.yml**




_**Q2:-**_



To improve the Stability we can impose a check where the developers can only do feature deployments once a week
There will only be production bug fixed that will go on-demand. That way we can increase the liabiility of system

The load time for changes should be immediate so the latest changes do reflect in production without failure, each pod should have same code and the cache should be updated too

The resource time allocation should be very less so as soon as the pod dies the new pod should replace it.

The change failure rate should be 0-2% so there is any failure order detected, it will raise flags.





_**Q3:-  **_

I tried to run the docker image on my local and it is working fine for me. kindly check it!
