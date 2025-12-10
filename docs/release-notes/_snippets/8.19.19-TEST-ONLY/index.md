## 8.19.19-TEST-ONLY [fleet-server-release-notes-8.19.19-TEST-ONLY]



### Features and enhancements [fleet-server-8.19.19-TEST-ONLY-features-enhancements]


* Support secrets in agent.download section of policy. [#6046](https://github.com/elastic/fleet-server/pull/6046) 
* Support secrets in fleet section of policy. [#6046](https://github.com/elastic/fleet-server/pull/6046) 
* Makes file storage size configurable. [#6046](https://github.com/elastic/fleet-server/pull/6046) 
* Accept secret references in policies in either inline or path formats. [#6046](https://github.com/elastic/fleet-server/pull/6046) 

  Elastic Agent policies can contain secret references in one of two formats: inline or path.
  With the inline format, the reference looks like this: `&lt;path&gt;: $co.elastic.secret{&lt;secret ref&gt;}`. 
  With the path format, the reference looks like this: `secrets.&lt;path&gt;.id:&lt;secret ref&gt;`.
  This change ensures that Fleet Server accepts secret references in policies in either format.
  



