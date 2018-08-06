
TARGETS=charbox.svg cluebox.svg counterbox.svg encounterbox.svg mythosbox.svg outerbox.svg resourcebox.svg \
	charbox.dxf cluebox.dxf counterbox.dxf encounterbox.dxf mythosbox.dxf outerbox.dxf resourcebox.dxf

THICKNESS=3 # mm

all: $(TARGETS)

clean:
	rm -f $(TARGETS)

%.svg : %.txt
	boxes TrayLayout2 --format=svg --h=$(HEIGHT) --input=$< --output=$@ --thickness=$(THICKNESS) --outside=0

%.dxf : %.txt
	boxes TrayLayout2 --format=dxf --h=$(HEIGHT) --input=$< --output=$@ --thickness=$(THICKNESS) --outside=0
