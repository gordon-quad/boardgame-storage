TARGETS=cardbox.svg chitbox.svg sidebox.svg test.svg \
	cardbox.dxf chitbox.dxf sidebox.dxf test.dxf

HEIGHT=22 # mm
THICKNESS=3.3 # mm

all: $(TARGETS)

clean:
	rm -f $(TARGETS)

%.svg : %.txt
	boxes TrayLayout2 --format=svg --h=$(HEIGHT) --input=$< --output=$@ --thickness=$(THICKNESS) --outside=0 --burn=0 --FingerJoint_play=-0.1

%.dxf : %.txt
	boxes TrayLayout2 --format=dxf --h=$(HEIGHT) --input=$< --output=$@ --thickness=$(THICKNESS) --outside=0 --burn=0 --FingerJoint_play=-0.1
