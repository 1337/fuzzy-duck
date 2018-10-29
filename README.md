# fuzzy-duck
Recommended reading for people with trouble writing code.

    does_he = False
    for step in range(1, 101):
        if does_he:
            player_id = 10 - step % 10
        else:
            player_id = step % 10

        if step % 15 == 0:
            msg = 'Does he?'
            does_he = not does_he
        elif step % 2 == 0:
            msg = 'Ducky fuzz'
        else:
            msg = 'Fuzzy duck'

        print '%s\t%s\t%s' % (step, player_id, msg)
