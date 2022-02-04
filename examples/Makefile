# cwm is a tool from the SWAP project
C=python2.7 ~/src/github.com/linkeddata/swap/cwm.py

# Make shapes from forms

profile-shapes-from-form.ttl : profileFormText.ttl profile-shape-seed.ttl ../tools/rules-form-to-shape.n3
	$C profileFormText.ttl profile-shape-seed.ttl --think=../tools/rules-form-to-shape.n3 --data --quiet > $@


# Make forms from shapes

shape-form-from-shapes.ttl : shacl-shacl.ttl rules-shape-to-form-2.n3
			$C shacl-shacl.ttl shape-seed.ttl --think=rules-shape-to-form-2.n3 > $@

contact-form-from-shapes.ttl : contacts-shapes.ttl rules-shape-to-form.n3
			$C contacts-shapes.ttl seed.ttl --think=rules-shape-to-form.n3 > $@
