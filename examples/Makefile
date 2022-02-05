# cwm is a tool from the SWAP project
C=python2.7 ~/src/github.com/linkeddata/swap/cwm.py
S=../../../solid/webid-profile/shapes
S2=../../solid-panes/src/dashboard/preferencesFormText.ttl
# Make shapes from forms
# (first is default)

both: contact-shapes-from-form.ttl  profile-shapes-from-form.ttl
	cat $< > $@

contact-shapes-from-form.ttl : contactFormText.ttl contact-shape-seed.ttl ../tools/rules-form-to-shape.n3
	$C contactFormText.ttl contact-shape-seed.ttl --think=../tools/rules-form-to-shape.n3 --data --quiet > $@

profile-shapes-from-form.ttl : profileFormText.ttl profile-shape-seed.ttl ../tools/rules-form-to-shape.n3
	$C profileFormText.ttl profile-shape-seed.ttl --think=../tools/rules-form-to-shape.n3 --data --quiet > $@

profileFormText.ttl : $S/profileFormText.ttl
	cp $S/profileFormText.ttl $@

# Make forms from shapes

shape-form-from-shapes.ttl : shacl-shacl.ttl rules-shape-to-form-2.n3
			$C shacl-shacl.ttl shape-seed.ttl --think=rules-shape-to-form-2.n3 > $@

contact-form-from-shapes.ttl : contacts-shapes.ttl rules-shape-to-form.n3
			$C contacts-shapes.ttl seed.ttl --think=rules-shape-to-form.n3 > $@
