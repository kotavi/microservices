The kubectl command-line interface can be used in different ways when working with Kubernetes objects. You can use imperative commands that operate directly on live objects in a cluster, or you can configure objects imperatively in a local file, or declaratively in directories of files. There are advantages and disadvantages to each method.

The simplest way to run tasks in a cluster is by using imperative commands, and this is typically what you would do with a development project. In a production environment, you might want to store object configuration files in a source control system, or operate on a directory of configuration files, and integrate with a review or change process.

Whatever you choose, it is important that you maintain a consistent approach when working with the same object, and do not mix approaches, or unexpected behavior can result.

The basic syntax of the command uses a verb, followed by the object type, a subtype if applicable, and the instance name.

`<verb> <objecttype> [<subtype>] <instancename>`

The example command here creates a service of subtype nodeport called myservice.

`kubectl create service nodeport myservice`

The tutorials in this course walk through many examples of how to use kubectl commands, and you can find more detailed information about kubectl in the Kubernetes documentation.


## Kubectl command reference

### Basic syntax

<verb> <objecttype> [<subtype>] <instancename> [flags]

Where the <verb> is an action such as: create, run, expose, autoscale, and so on.

<objecttype> is the object type, such as a service. Some objects have subtypes that you can specify with the create command. For example, a service has subtypes of ClusterIP, LoadBalancer, NodePort, and so on. Use the -h flag to find the arguments and flags that are supported by a specific subtype. Types and subtypes are case-sensitive.

<instancename> specifies the name of the object. Names are also case-sensitive. If you omit the name, details for all resources of the specified type are displayed.

Optionally, you can specify flags that do various functions. For example, you can use the -s flag to specify the address and port of the Kubernetes API server. Flags that you specify from the command line override default values and any corresponding environment variables.

To answer quiz questions about kubectl commands in this course, you only need to enter the verb, object type, and subtype, if applicable. You do not need to specify an instance name or any optional flags with the command.

For a complete list of kubectl commands, see the Kubernetes documentation.

#### Some useful commands

Get help with kubectl commands:

`$ kubectl help`

Get the state of your cluster:

`$ kubectl cluster-info`

Get all the Nodes of your cluster:

`$ kubectl get nodes -o wide`

Get information about the Pods of your cluster:

`$ kubectl get pods -o wide`

Get information about the Replication Controllers of your cluster:

`$ kubectl get rc -o wide`

Get information about the Services of your cluster:

`$ kubectl get services`

Get full configuration information about a Service:

`$ kubectl get service <instancename> -o json`

Get the IP address of a Pod:

`$ kubectl get pod <instancename> -template={{.status.podIP}}`

Delete a Pod:

`$ kubectl delete pod NAME`

Delete a Service:

`$ kubectl delete service <instancename>`

### Useful links

kubectl reference - https://kubernetes.io/docs/reference/

kubectl cheat sheet - https://kubernetes.io/docs/user-guide/kubectl-cheatsheet/