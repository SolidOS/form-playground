C=python2.7 /Users/timbl/src/github.com/linkeddata/swap/cwm.py

# Make forms from shapes
contact-form-from-shapes.ttl : contacts-shapes.ttl rules-shape-to-form.n3
			$C contacts-shapes.ttl seed.ttl --think=rules-shape-to-form.n3 > $@
