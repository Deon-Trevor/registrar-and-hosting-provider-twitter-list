# registrar-and-hosting-provider-twitter-list
A list of registrars and hosting providers' twitter handles (if they have one)

The list is still pretty small, please feel free contribute. The list is a simple json (json always make life easier!!!) like:

```
{
  "namecheap": "@Namecheap",
  "godaddy": "@GoDaddy",
  ...
}
```

# Usecase
The idea for this list is [PhishGalore](https://twitter.com/phishgalore/status/1467900400221179913)'s. His idea is to use this in a twitter bot like [Phisher Of Man](https://twitter.com/PhisherOfMan) to report phishing, malware, etc. [Phisher Of Man](https://twitter.com/PhisherOfMan)'s current version needs me manually look for a registrar/hosting provider's handle and feed it the script like:

```
Enter the target
> @Sync_Pundit

Enter the phish
> //syncpundit.com                

Enter the hosting provider or registrar
> @Namecheap

Enter the asn
> ASS1234

Enter the ip
> 127.0.0.1
```

With this list i can just call the desired registrar/namecheap as easy as:

```
$ python3 phisher-of-man.py namecheap

Enter the target
> @Sync_Pundit

Enter the phish
> //syncpundit.com                

... adding @Namecheap to the report ...

Enter the asn
> ASS1234

Enter the ip
> 127.0.0.1
```

# Further development
Soon we'll be adding the ASNs
